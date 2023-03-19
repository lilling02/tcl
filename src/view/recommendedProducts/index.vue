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

/*  产品推荐的title */
.recommendedProducts__title {
    box-sizing: content-box;
    display: flex;
    justify-content: space-between;
    margin-bottom: 1rem;
}

.recommendedProducts__title>:first-child {
    font-size: 2vw;
}

.recommendedProducts__title>:nth-child(2) {
    display: flex;
    flex-direction: column-reverse;
}

/* 去掉.recommendedProducts__title:nth-child(2) 中a标签的默认样式 */
.recommendedProducts__title>:nth-child(2) a {
    font-size: 0.8rem;
    text-decoration: none;
    color: #000;
}


/* 产品推荐的content */
.recommendedProducts__content {
    padding: 0;
    margin-top: 2vw;
    display: flex;
}

.recommendedProducts__content ul {
    padding: 0;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    width: 100%;
}

.recommendedProducts__content ul li {
    box-sizing: content-box;
    position: relative;
    width: 49.3%;
    height: max-content;
    overflow: hidden;
    margin-bottom: 1vw;
    cursor: pointer;
}

.recommendedProducts__content--text {
    position: absolute;
    bottom: -1vw;
    box-sizing: border-box;
    width: 100%;
    padding: 1vw;
}

.recommendedProducts__content--text p {
    color: rgb(255, 255, 255);
    font-size: 1.5vw;
}


/* 遮罩层内的内容 */
.recommended-products-mask {
    display: flex;
    margin-top: 0.5vw;
    justify-content: space-between;
    height: 0.8em;
    opacity: 0;
}

/* p标签的默认样式里面是自带padding 和 margin的 @ 2023/3/18 */
.recommended-products-mask p {
    padding: 0;
    margin: 0;
    font-size: 12px;
    opacity: .6;
    color: rgb(255, 255, 255);
}

.recommended-products-mask a {
    font-size: 12px;
    text-decoration: none;
    color: rgb(255, 255, 255);
}

/* 处理推荐产品的图片 */
.recommendedProducts__content--img {
    overflow: hidden;
}

.recommendedProducts__content--img img {
    width: 100%;
    object-fit: scale-down;
}

/* 处理鼠标移入的时候的动画 */
.recommendedProducts__content ul li:hover img {
    transform: scale(1.1);
    transition: all 0.5s;
    z-index: -1;
    /* img做动画的时候会造成他的图层升高导致遮住下面的东西 */
}

/* 处理鼠标移入的时候的文本的动画 */
.recommendedProducts__content ul li:hover .recommendedProducts__content--text {
    transform: translateY(-25%);
    transition: all 0.7s;
    z-index: 1;
}

/* 处理鼠标移入的时候的遮罩层的动画 */
.recommendedProducts__content ul li:hover .recommended-products-mask {
    opacity: 1;
    transition: all 0.7s;
}



/* 鼠标移出的动画 */
.recommendedProducts__content ul li img {
    z-index: 0;
    transform: none;
    transition: all 0.5s;
}

.recommendedProducts__content ul li .recommendedProducts__content--text {
    z-index: 1;
    transform: translateY(0);
    transition: all 0.7s;
}

.recommendedProducts__content ul li .recommended-products-mask {
    opacity: 0;
    transition: all 0.7s;
}


/* 设计产品列表里面两个特殊的样式 */
#recommended-Products__left {
    box-sizing: content-box;
    width: 36%;
    height: max-content;
}

#recommended-Products__left img {
    width: 100%;
    height: 100%;
    object-fit: fill;
}

#recommended-Products__right {
    box-sizing: content-box;
    width: 62.6%;
    height: max-content;
}

#recommended-Products__right img {
    width: 100%;
    height: 100%;
}
</style>