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
            <div class="row">
                <div id="carouselExampleFade" class="carousel slide carousel-fade" data-bs-ride="carousel">
                    <div class="carousel-inner">
                        <div class="carousel-item active d-flex justify-content-center">
                            <div  class="card border-0"  style="width: 30rem; height: 18rem">
                                <div class="card-body d-flex justify-content-center flex-column text-start">
                                    <div>
                                        <h5 class="card-title pb-3 colortext">I'ts choise of qualioty for people with special needs</h5>
                                        <h6 class="card-subtitle mb-2 text-muted pb-3">I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.</h6>
                                    </div>
                                    <div class="d-flex align-items-center">
                                        <div class="pe-3">
                                            <img class="rounded-circle" src="../assets/img/testimonial-avata-04.jpg" width="50" alt="">
                                        </div>
                                        <div class="text-start ">
                                            <div class="colortext"><strong>FLORENCE THEMES</strong></div>
                                            <div><span>/Multimedia Admin</span></div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="carousel-item d-flex justify-content-center" v-for="element in listaTestimonial" :key="element.name">
                            <div  class="card border-0 " style="width: 30rem; height: 18rem">
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
                        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleFade" data-bs-slide="prev">
                            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                            <span class="visually-hidden">Previous</span>
                        </button>
                        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleFade" data-bs-slide="next">
                            <span class="carousel-control-next-icon" aria-hidden="true"></span>
                            <span class="visually-hidden">Next</span>
                        </button>
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
                    title: "Nice Community, and constant help for all client",
                    paragraph: "I need get a certification for English proficiency ad MaxCoach is my best choise. Their tutors are smart and professional when dealing with students.",
                    name: "ARTUR PORTUA",
                    job: "Social Media Manager",
                    img: "03"
                },
                {
                    title: "Beatiful ambience, and friendly custumer care",
                    paragraph: "I need get a certification for English proficiency ad MaxCoach is my best choise. Their tutors are smart and professional when dealing with students.",
                    name: "NATASHA MILIKOVA",
                    job: "Data Analyst",
                    img: "04"
                },
                {
                    title: "Service 24h, and just with only a click on the page, teh custumer service is ready for  you",
                    paragraph: "I need get a certification for English proficiency ad MaxCoach is my best choise. Their tutors are smart and professional when dealing with students.",
                    name: "MIRKO SANTOS",
                    job: "Graphic Designer",
                    img: "05"
                },
                {
                    title: "Professional team of specialists and appasionate mentors at reach",
                    paragraph: "I need get a certification for English proficiency ad MaxCoach is my best choise. Their tutors are smart and professional when dealing with students.",
                    name: "CARMEN CONSOLI",
                    job: "Economic",
                    img: "06"
                },
                {
                    title: "Professional team of specialists and appasionate mentors at reach",
                    paragraph: "I need get a certification for English proficiency ad MaxCoach is my best choise. Their tutors are smart and professional when dealing with students.",
                    name: "CARLOS RAMIRES",
                    job: "Barber",
                    img: "07"
                },
                {
                    title: "Professional team of specialists and appasionate mentors at reach",
                    paragraph: "I need get a certification for English proficiency ad MaxCoach is my best choise. Their tutors are smart and professional when dealing with students.",
                    name: "TIFFANY CHARLOT",
                    job: "Doctor",
                    img: "08"
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
        color: #1eae96;
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