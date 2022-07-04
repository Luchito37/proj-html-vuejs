<template>
    <div class="section">
        <div class="container">
            <div class="row px-5">
                <div class="col px-5 mb-5 spacing">
                    <div class="px-5 colortext"><h5>Let's Dream Big Togeter</h5></div>
                    <div class="px-5">
                        <h3>Explore How can I help you</h3>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col d-flex justify-content-center mx-3">
                    <div class="card mx-3 shadow-lg" v-for="element in caratteristicheCard" :key="element.img" style="width: 18rem;">
                        <img :src="require('../assets/img/home-business-service-slide-'+ element.img +'-480x298.jpg')" class="card-img-top" alt="...">
                        <div class="card-body">
                            <div><h3>{{element.title}}</h3></div>
                            <p class="card-text">{{element.paragraph}}</p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col">
                    <span class="fs-1"> . <span class="text-secondary fs-2">. .</span></span>
                </div>
            </div>
        </div>
    </div>
</template>


<script>

export default {
    data(){
        return {
            caratteristicheCard: [
                {
                    title: "Consulting Training",
                    paragraph: "With a coach addressing multiple issues that are off balance, affecting your business in various unconsidered ways.",
                    img: "01"
                },
                {
                    title: "Real Deal Coaching",
                    paragraph: "Bring an exceptionally powerfull opportunity. Being able to accept, to work with that opportunity.",
                    img: "02"
                },
                {
                    title: "Advisor Training Program",
                    paragraph: "Getting high quality, entrepreneur mindset driven on line business coaching, is what is needed.",
                    img: "03"
                },

            ]
        }
    }
}

</script>

<style scoped lang="scss">
    .section{
        margin-top: 100px;
        background-color: #eceeef;
    }
    .spacing{
        margin-top: 100px;
    }
    .colortext{
        color: #1eae96;
    }
</style>