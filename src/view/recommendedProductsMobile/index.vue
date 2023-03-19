<script setup>

</script>

<template>
    <div class="recommendedProducts">
            <div class="recommendedProducts__title">
                <div>推荐产品</div>
                <div>
                    <a href="">查看更多</a>
                </div>
            </div>
            <div class="recommendedProducts__content">
                <div class="recommendedProducts__content--carousel">
                    <div class="block text-center">
                        <el-carousel height="69vw">
                            <!-- 跑马灯内容的区域 -->
                        <el-carousel-item>
                                <img src="https://www.tcl.com/content/dam/brandsite/region/china/cnx/home/assets/product1.jpg" alt="">
                        </el-carousel-item>
                        <el-carousel-item>
                                <img src="https://www.tcl.com/content/dam/brandsite/region/china/cnx/home/assets/product1.jpg" alt="">
                        </el-carousel-item>
                        </el-carousel>
                        <span class="demonstration">领曜QD-MiniLED智屏X11</span>
                    </div>
                </div>

                <!-- 跑马灯效果尾部 商品推荐头部 -->
                <ul>
                    <li>
                        <div class="recommendedProducts__content--text">
                            <p>领曜QD-MiniLED智屏X11</p>
                            <div class="recommended-products-mask">
                                <p>不灼屏 更绚丽</p>
                                <a href="">
                                    了解更多
                                    <i>></i>
                                </a>
                            </div>
                        </div>
                        <div class="recommendedProducts__content--img">
                            <img
                                src="https://www.tcl.com/content/dam/brandsite/region/china/cnx/home/assets/product1.jpg">
                        </div>
                    </li>
                    <li>
                        <div class="recommendedProducts__content--text">
                            <p>领曜QD-MiniLED智屏X11</p>
                            <div class="recommended-products-mask">
                                <p>不灼屏 更绚丽</p>
                                <a href="">
                                    了解更多
                                    <i>></i>
                                </a>
                            </div>
                        </div>
                        <div class="recommendedProducts__content--img">
                            <img
                                src="https://www.tcl.com/content/dam/brandsite/region/china/cnx/home/assets/product1.jpg">
                        </div>
                    </li>

                    <!-- 样式里偏小的一个,左边 -->
                    <li id="recommended-Products__left">
                        <div class="recommendedProducts__content--text ">
                            <p>领曜QD-MiniLED智屏X11</p>
                            <div class="recommended-products-mask">
                                <p>不灼屏 更绚丽</p>
                                <a href="">
                                    了解更多
                                    <i>></i>
                                </a>
                            </div>
                        </div>
                        <div class="recommendedProducts__content--img">
                            <img
                                src="https://www.tcl.com/content/dam/brandsite/region/china/cnx/home/assets/product3.jpg">
                        </div>
                    </li>

                    <!-- 样式里面偏大的一个,右边 -->
                    <li id="recommended-Products__right">
                        <div class="recommendedProducts__content--text">
                            <p>领曜QD-MiniLED智屏X11</p>
                            <div class="recommended-products-mask">
                                <p>不灼屏 更绚丽</p>
                                <a href="">
                                    了解更多
                                    <i>></i>
                                </a>
                            </div>
                        </div>
                        <div class="recommendedProducts__content--img">
                            <img src="https://www.tcl.com/content/dam/brandsite/region/china/cnx/home/assets/c163.jpg">
                        </div>
                    </li>
                    <li>
                        <div class="recommendedProducts__content--text">
                            <p>领曜QD-MiniLED智屏X11</p>
                            <div class="recommended-products-mask">
                                <p>不灼屏 更绚丽</p>
                                <a href="">
                                    了解更多
                                    <i>></i>
                                </a>
                            </div>
                        </div>
                        <div class="recommendedProducts__content--img">
                            <img
                                src="https://www.tcl.com/content/dam/brandsite/region/china/cnx/home/assets/product1.jpg">
                        </div>
                    </li>
                    <li>
                        <div class="recommendedProducts__content--text">
                            <p>领曜QD-MiniLED智屏X11</p>
                            <div class="recommended-products-mask">
                                <p>不灼屏 更绚丽</p>
                                <a href="">
                                    了解更多
                                    <i>></i>
                                </a>
                            </div>
                        </div>
                        <div class="recommendedProducts__content--img">
                            <img
                                src="https://www.tcl.com/content/dam/brandsite/region/china/cnx/home/assets/product1.jpg">
                        </div>
                    </li>
                </ul>

            </div>
        </div>
</template>

<style scoped>
/*  */
.recommendedProducts{
    margin: 0 auto;
    width: 92vw;
}
.recommendedProducts__title {
    font-size: 6.5vw;
    box-sizing: content-box;
    display: flex;
    justify-content: space-between;
    margin-bottom: 8.5vw;
}

.recommendedProducts__title>:nth-child(2) {
    display: flex;
    flex-direction: column-reverse;
}

/* 去掉.recommendedProducts__title:nth-child(2) 中a标签的默认样式 */
.recommendedProducts__title>:nth-child(2) a {
    font-size: 4.3vw;
    text-decoration: none;
    color: #000;
}

/* element跑马灯效果 */

.demonstration {
    box-sizing: content-box;
    display: block;
    margin-top: 2.25vw;
    font-size: 5vw;
}

.el-carousel__item div{
  height: 100%;
  width: 100%;
}
.el-carousel__item img {
  object-fit: cover;
  height: 100%;
  width: 100%;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}

/* 跑马灯结束商品推荐内容 */
.recommendedProducts__content ul{
    display: flex;
    justify-content:space-between;
    flex-wrap: wrap;
    width: 100%;
    margin-top: 5vw;
    overflow: hidden;
}

li {
    box-sizing: border-box;
    position: relative;
    width: 48.5%;
    height: max-content;
    margin-bottom: 10vw;
    cursor: pointer;
}

.recommendedProducts__content--img img {
    width: 100%;
    height: 45vw;
    object-fit: cover;
}

.recommended-products-mask {
    display: none;
}

.recommendedProducts__content--text {
    position: absolute;
    bottom: -5vw;
}

.recommendedProducts__content--text p{
    font-size: 3.5vw;
    white-space: nowrap; /* 避免换行 */
    overflow: hidden; /* 超出部分隐藏 */
    text-overflow: ellipsis; /* 显示省略号 */
}
</style>