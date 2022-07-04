<template>
    <div class="section">
        <div class="container">
            <div class="row">
                <div class="col d-flex justify-content-center align-items-center">
                    <img src="../assets/img/circle.png" width="100"  alt="">
                </div>
                <div class="col d-flex flex-column justify-content-center">
                    <div class="mb-4">
                        <h1>Subscribe <span class="colortext">Newsletters</span></h1>
                        <p>Enter your email address to register to our newsletter subscription delivered on a regular basis! </p>
                    </div>
                    <div>
                        <nav class="d-inline-block">
                            <div class="d-flex" :class="questionCliccata === true ? 'd-none' : 'd-inline-block'">
                                <input class="bgInput border border-0 rounded-start py-2 px-1" type="search" placeholder="Enter your email" aria-label="Search">
                                <button class="border border-0 bgbuttom rounded-end text-white px-3" @click="impostaVisibilita" type="submit">Subscribe</button>
                            </div>
                            <div>
                                <h3 class="colortext" :class="questionCliccata === true ? 'd-inline-block' : 'd-none'">YOU'RE ALREADY SUB!</h3>
                            </div>
                        </nav>
                    </div>
                </div>
                <div class="col d-flex justify-content-center align-items-center bgImgcube">
                    <img src="../assets/img/maxcoach-shape-02.png" width="100" alt="">
                </div>
            </div>
        </div>
    </div>
</template>


<script>

export default {
    data(){
        return {
            questionCliccata: false,
        }
    },
    methods:{
        impostaVisibilita(){
            return this.questionCliccata = true;
        },
    },
}

</script>



<style scoped lang="scss">
    .section{
        margin: 80px 0;
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
    .bgInput{
        background-color: #eceeef;
        width: 350px;
        
    }
    .bgImgcube{
        background-image: url(../assets/img/maxcoach-shape-09.png);
        background-position: bottom;
        background-repeat: no-repeat;
        width: 180px;
        height: 180px;
        z-index: 0;
    }
    
</style>