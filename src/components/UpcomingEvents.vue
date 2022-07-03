<template>
    <div class="section">
        <div class="container">
            <div class="row px-5">
                <div class="col px-5 mb-5 spacing">
                    <div class="px-5 colortext"><h5>Wonna Trasform your life?</h5></div>
                    <div class="px-5">
                        <h1>Upcoming events</h1>
                    </div>
                </div>
            </div>
            <div class="row row-cols-2">
                <div class="col d-flex justify-content-center mb-4" v-for="element in listaEventi" :key="element.date">
                    <div class="card d-flex bgCard border-0" style="width: 35rem;">
                        <div class="card-body d-flex justify-content-between align-items-center">
                            <div class="text-start">
                                <h6 class="card-subtitle mb-2 text-muted"><i class="fa-solid fa-location-dot px-2"></i>{{element.location}}</h6>
                                <h5 class="card-title">{{element.paragraph}}</h5>
                            </div>
                            <div>
                                <div>
                                    <h1 class="colortext">{{element.date}}</h1>
                                    <h6>{{element.mounth}}</h6>
                                </div>
                                <div>
                                    <button type="button" class="btn bgbuttom text-white">Get ticket</button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row px-5">
                <div class="col px-5 mb-5 spacing">
                    <div class="px-5"><h5>Excited about our event? <span class=" colortext text-decoration-underline">View all events <i class="fa-solid fa-arrow-right-long"></i></span></h5></div>
                </div>
            </div>
            
        </div>
    </div>
</template>


<script>

export default {
    data(){
        return {
            listaEventi: [
                {
                    date: "22",
                    paragraph: "Story Telling Workshop",
                    location: "Texas, US",
                    mounth: "NOV"
                },
                {
                    date: "10",
                    paragraph: "Painting Art Contest 2022",
                    location: "New York, US",
                    mounth: "OCT"
                },
                {
                    date: "23",
                    paragraph: "International Art Fair 2020",
                    location: "Humburg, Germany",
                    mounth: "NOV"
                },
                {
                    date: "15",
                    paragraph: "Street Performance: Call for Artist",
                    location: "Illinois, US",
                    mounth: "DEC"
                },
                {
                    date: "22",
                    paragraph: "Consumer food Safety Education Conference",
                    location: "Illinois, US",
                    mounth: "NOV"
                },
                {
                    date: "12",
                    paragraph: "How meditation improve your mental healt?",
                    location: "Dubai",
                    mounth: "AUG"
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
</style>