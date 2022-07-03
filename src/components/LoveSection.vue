<template>
    <div class="section">
        <div class="container">
            <div class="row px-5">
                <div class="col px-5 mb-5 spacing">
                    <div class="px-5 colortext"><h5>People are praising Maxcoach</h5></div>
                    <div class="px-5">
                        <h1>Whate make they love us?</h1>
                    </div>
                </div>
            </div>
            <div class="row row-cols-3">
                <div class="col d-flex mb-4" v-for="element in listaTestimonial" :key="element.name">
                    <div class="card border-0" style="width: 30rem; height: 18rem">
                        <div class="card-body d-flex justify-content-center flex-column text-start">
                            <div>
                                <h5 class="card-title pb-3 colortext">{{element.title}}</h5>
                                <h6 class="card-subtitle mb-2 text-muted pb-3">{{element.paragraph}}</h6>
                            </div>
                            <div class="d-flex align-items-center">
                                <div class="pe-3">
                                    <img class="rounded-circle" :src="require('../assets/img/testimonial-avata-'+ element.img +'.jpg')" width="50" alt="">
                                </div>
                                <div class="text-start ">
                                    <div class="colortext"><strong>{{element.name}}</strong></div>
                                    <div><span>/{{element.job}}</span></div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col">
                    <span class="font"> . <span class="text-secondary font">. .</span></span>
                </div>
            </div>
            
        </div>
    </div>
</template>


<script>

export default {
    data(){
        return {
            listaTestimonial: [
                {
                    title: "High level of efficiency and scientific teching methods",
                    paragraph: "I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
                    name: "MINA HOLLACE",
                    job: "Freelancer",
                    img: "01"
                },
                {
                    title: "Professional team of specialists and appasionate mentors at reach",
                    paragraph: "I need get a certification for English proficiency ad MaxCoach is my best choise. Their tutors are smart and professional when dealing with students.",
                    name: "MADLEY PONDOR",
                    job: "IT Specialists",
                    img: "02"
                },
                {
                    title: "I'ts choise of qualioty for people with special needs",
                    paragraph: "I'm very strict person so I require everething to be organized and neat. Then, I'll be able to make things right and shine. MaxCoach guys just got me.",
                    name: "FLORENCE THEMES",
                    job: "Multimedia Admin",
                    img: "04"
                },

            ]
        }
    }
}

</script>




<style scoped lang="scss">
    .section{
        padding: 100px 0;
        background-color: #eceeef
    }
    .colortext{
        color: #343142;
    }
    .bgCard{
        background-color: #eceeef;
    }
    .bgbuttom{
        background-color: #1eae96;

        &:hover{
            background-color: #61e6d2;
            border: solid 1px #61e6d2 ;
        }
    }
    .font{
        font-size: 80px;
    }
</style>