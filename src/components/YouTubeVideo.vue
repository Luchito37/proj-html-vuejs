<template>
    <div class="section bgImgAvatar">
        <div class="container spacing">
            <div class="row row-cols-md-2">
                <div class="col d-flex position-relative">
                    <div class="position-absolute top-100 start-0 translate-middle bgImgcube"></div>
                    <div class="card text-white bgTube">
                        <img src="../assets/img/home-business-video-poster-670x450.jpg" class="card-img" alt="...">
                        <div class="card-img-overlay d-flex justify-content-center align-items-center">
                                <img src="../assets/img/icon-youtube-play.png" alt="">
                        </div>
                    </div>
                </div>
                <div class="col text-white text-start ">
                    <div>
                        <div>
                            <h1>To Thrive in Buiness Today, You'll Need a Good Plan</h1>
                        </div>
                        <div>
                            <ul class="text-start list-unstyled pt-4" v-for="element in listaDomande" :key="element.question">
                                <li>
                                    <h5 @click="impostaVisibilita" >{{element.question}}</h5>
                                    <h6 @click="impostaTrasparenza"  class="text-secondary"  :class="questionCliccata === true ? 'd-inline-block' : 'd-none'">{{element.answer}} <i class="fa-solid fa-arrow-up-long colortext border-bottom"></i></h6>
                                </li>
                                <hr>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<script>

export default {
    data(){
        return {
            listaDomande: [
                {
                    question: "How can help you?" ,
                    answer: "How many courses you have been on, using however many techniques and methods. Unless you have come to realize teh value of mindset, then you have to understand how succes comes."
                },
                {
                    question: "Why would I need a business COACH?" ,
                    answer: "How many courses you have been on, using however many techniques and methods. Unless you have come to realize teh value of mindset, then you have to understand how succes comes."
                },
                {
                    question: "What is one-on-one coaching?" ,
                    answer: "How many courses you have been on, using however many techniques and methods. Unless you have come to realize teh value of mindset, then you have to understand how succes comes."
                },

            ],
            questionCliccata: false,
            answerNascosta: false
        }
    },
    methods:{
        impostaVisibilita(){
            return this.questionCliccata = true;
        },
        impostaTrasparenza(){
            return this.questionCliccata = false
        }
    },
}

</script>




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
    .bgTube{
    justify-content: center;
    background-color: #ffffff00;
    border: none;
    }
</style>