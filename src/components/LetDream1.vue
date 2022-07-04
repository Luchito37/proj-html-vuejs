<template>
    <div class="section">
        <div class="container">
            <div class="row px-5">
                <div class="col px-5 mb-5">
                    <div class="px-5 colortext"><h5>Let's Dream Big Togeter</h5></div>
                    <div class="px-5">
                        <h3>We are pioneers of the digital approach, using leading-edge technology to simplify procedures
                            and apply executive coaching in the new age of digitalization.</h3>
                    </div>
                </div>
            </div>
            <div class="row row-cols-3 px-5">
                <div class="col d-flex mb-5 px-5" v-for="element in listaPeculiarita" :key="element.img">
                    <div>
                        <img :src="require('../assets/img/icon-'+ element.img +'.png')" width="40" alt="">
                    </div>
                    <div class="text-start px-4">
                        <div>
                            <h4>{{element.title}}</h4>
                        </div>
                        <div>
                            <div>{{element.paragraph}}</div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col d-flex justify-content-center">
                    <div class="p-3">
                        <button type="button" class="btn border-secondary colortext">Get started today</button>
                    </div>
                    <div class="p-3">
                        <button type="button" class="btn bgbuttom text-white">Get started today</button>
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
            listaPeculiarita: [
                {
                    title: "One to One",
                    paragraph: "Get the necessary clarity about the current state to help you improve your game.",
                    img: "people"
                },
                {
                    title: "Anywhere",
                    paragraph: "Access to valuable and portable program which allow you to setup and live anywhere you want.",
                    img: "anywhere"
                },
                {
                    title: "On Time",
                    paragraph: "Punctuality is yor top priority beacause it's an essential criteria to assess a program quality.",
                    img: "time"
                },
                {
                    title: "Online Courses",
                    paragraph: "Online business coaching now offers you a very powerfull way to empower your business into success.",
                    img: "online"
                },
                {
                    title: "Consulting",
                    paragraph: "You will get a clear sense of direction for your business, throught assessment and faster results.",
                    img: "consulting"
                },
                {
                    title: "Self Develoapment",
                    paragraph: "Business coaching often keep your focus and develop you both in a professional and personal way.",
                    img: "development"
                },

            ]
        }
    }
}

</script>


<style scoped lang="scss">
    .section{
        margin-top: 100px;
    }
    .colortext{
        color: #1eae96;
    }
    .bgbuttom{
        background-color: #1eae96;

        &:hover{
            background-color: #61e6d2;
            border: solid 1px #61e6d2 ;
        }
    }
</style>
