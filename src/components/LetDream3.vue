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
            <div class="row row-cols-4">
                <div class="col d-flex" v-for="element in caratteristicheCard" :key="element.img">
                    <div class="card text-white">
                        <img :src="require('../assets/img/stock-full-hd-'+ element.img +'-443x600.jpg')" class="card-img" alt="...">
                        <div class="card-img-overlay d-flex justify-content-end flex-column align-items-start text-start ombre">
                            <h5 class="card-title colortext">${{element.price}}</h5>
                            <p class="card-text">{{element.paragraph}}</p>
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
            caratteristicheCard: [
                {
                    price: "40.00",
                    paragraph: "Learn to Write as a Professional Author.",
                    img: "01"
                },
                {
                    price: "FREE",
                    paragraph: "Customer-centric Info-tech Strategies.",
                    img: "03"
                },
                {
                    price: "19.00",
                    paragraph: "Open Programmming Courses for Everyone: Python.",
                    img: "04"
                },
                {
                    price: "26.00",
                    paragraph: "Academic Listening and Note-taking .",
                    img: "06"
                },

            ]
        }
    }
}

</script>



<style scoped lang="scss">
    .section{
        margin: 80px 0;
    }
    .spacing{
        margin-top: 100px;
    }
    .colortext{
        color: #1eae96;
    }
    .ombre{
        box-shadow: inset 0px -100px 20px 0px #000000ad;
    }
</style>