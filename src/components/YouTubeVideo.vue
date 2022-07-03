<template>
    <div class="section bgImgAvatar">
        <div class="container spacing">
            <div class="row row-cols-2">
                <div class="col d-flex position-relative">
                    <div class="position-absolute top-100 start-0 translate-middle bgImgcube"></div>
                    <div class="card text-white ">
                        <img src="../assets/img/home-business-video-poster-670x450.jpg" class="card-img" alt="...">
                        <div class="card-img-overlay d-flex justify-content-center align-items-center">
                                <img src="../assets/img/icon-youtube-play.png" width="80" alt="">
                        </div>
                    </div>
                </div>
                <div class="col text-white text-start ">
                    <div>
                        <div>
                            <h1>To Thrive in Buiness Today, You'll Need a Good Plan</h1>
                        </div>
                        <div>
                            <ul class="text-start">
                                <li>How can help you?</li>
                                <hr>
                                <li>Why would I need a business COACH?</li>
                                <hr>
                                <li>What is one-on-one coaching?</li>
                                <hr>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>




<style scoped lang="scss">
    .section{
        background-color: #343142;
        padding: 100px 0;
    }
    .bgImgAvatar{
        background-image: url(../assets/img/background-map-dots-top-right-transparent.png);
        background-position: right;
        background-size: contain;
        background-repeat: no-repeat;
    }
    .bgImgcube{
        background-image: url(../assets/img/maxcoach-shape-07-100x100.png);
        background-position: bottom;
        background-repeat: no-repeat;
        width: 180px;
        height: 180px;
        z-index: 0;
    }
    .spacing{
        padding: 0 100px;
    }
    .colortext{
        color: #1eae96;
    }
</style>