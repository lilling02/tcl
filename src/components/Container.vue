<script setup>
import { computed,reactive } from '@vue/reactivity';
import RecommenedProducts from '../view/recommendedProducts/index.vue'
import RecommendedProductsMobile from '../view/recommendedProductsMobile/index.vue'
import { onUnmounted, ref,watch } from 'vue';

const state = reactive({
  isMobile: window.innerWidth < 785 ? true : false,
});

const onResize = () => {
  if (window.innerWidth < 785) {
    state.isMobile = true;
  } else {
    state.isMobile = false;
  }
  console.log(state.isMobile);
};

// 监听窗口大小变化
window.addEventListener('resize',onResize);

// x组件销毁时,移除监听
onUnmounted(()=>{
    window.removeEventListener('resize',onResize);
})

</script>

<template>
    <div class="container">
        <!-- 网页端 -->
        <RecommenedProducts v-if="!state.isMobile"></RecommenedProducts>

        <!-- 移动端 -->
        <RecommendedProductsMobile v-if="state.isMobile"></RecommendedProductsMobile>
    </div>
</template>

<style >
    /* 写一个1920的媒体查询 */
@media screen and (min-width: 1900px) {
    .container {
        margin: 0 auto;
        width: 1200px;
        height: 1200px;
    }
}

/* 写一个大于960小于1920的媒体查询 */
@media screen and (min-width: 960px) and (max-width: 1900px) {
    .container {
        margin: 0 auto;
        width: 960px;
        height: 960px;
    }
}

/* 写一个大于785 小于 960的媒体查询 */
@media screen and (min-width: 785px) and (max-width: 960px) {
    .container {
        margin: 0 auto;
        width: 785px;
        height: 785px;
    }
}

</style>