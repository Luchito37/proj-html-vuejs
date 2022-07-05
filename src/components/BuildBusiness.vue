<template>
    <div class="bgSection">
        <div class="container">
            <div class="row row-cols-lg-2 row-cols-sm-1 align-items-center  justify-content-sm-center">
                <div class="col-lg-4  col-sm-6 d-flex flex-column text-lg-start text-md-center px-3">
                    <div class="colortext">
                        <h5>New Challenges, New Skills</h5>
                    </div>
                    <div>
                        <h1>BUILD YOUR OWN LIFE COACHING BUSINESS</h1> 
                    </div>
                    <div>
                        <p>Whole-Life Business Coaching for committed entrepreneurs</p>
                    </div>
                    <div>
                        <button type="button" class="btn bgbuttom text-white">Get started today</button>
                    </div>
                </div>
                <div class="col px-4">
                    <div class="bgImgAvatar">
                        <img src="../assets/img/home-business-hero-avatar.png" width="400" alt="">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>

export default {
}
</script>


<style scoped lang="scss">
    .bgSection{
        background-color: #ecf2f9;
    }
    .bgImgAvatar{
        background-image: url(../assets/img/home-business-hero-global-image.png);
        background-position: center;
        background-size: contain;
        background-repeat: no-repeat;
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