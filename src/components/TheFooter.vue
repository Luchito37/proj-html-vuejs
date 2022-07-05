<template>
    <div class="section position-relative">
        <div class="container">
            <div class="row row-cols-2">
                <div class="col text-start text-secondary">
                    <div>
                        <h3 class="text-white"><strong>Address</strong></h3>
                        <p>382 NE 191st St # 87394 Miami, FL 33179-3899</p>
                        <p>+1(305)547-9909 (9am - 5pm EST,Monday - Friday)</p>
                        <p>support@maxcoach.com</p>
                    </div>
                    <div class="d-flex fs-3"> 
                        <div class="pe-4">
                            <i class="fa-brands fa-linkedin"></i>
                        </div>
                        <div class="pe-4">
                            <i class="fa-brands fa-instagram"></i>
                        </div>
                        <div class="pe-4">
                            <i class="fa-brands fa-twitter"></i>
                        </div>
                        <div>
                            <i class="fa-brands fa-facebook-square"></i>
                        </div>
                    </div>
                </div>
                <div class="col text-secondary d-flex pe-5 text-start">
                    <div class="pe-5">
                        <h3 class="text-white">Explosure</h3>
                        <ul class="list-unstyled" v-for="element in listaExplosure" :key="element.date">
                            <li>{{element}}</li>
                        </ul>
                    </div>
                    <div class="pe-5">
                        <h3 class="text-white">Explosure</h3>
                        <ul class="list-unstyled" v-for="element in listaInformation" :key="element.date">
                            <li>{{element}}</li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="row mt-5">
                <div class="col text-white px-5  spacing">
                    <div class="px-5"><h6 class="text-secondary">© 2020 Maxcoach. All Right Reserved</h6></div>
                </div>
                
                    <div class=" rounded-circle bg-arrow d-flex align-items-center justify-content-center fixed-bottom">
                        <div>
                            <a href="#"><i class="fa-solid fa-arrow-up-long"></i></a>
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
            listaExplosure: [
                "Start Here",
                        "Blog",
                        "About us",
                        "Succes story",
                        "Courses",
                        "Contact us"
            ],
            listaInformation:[
                "Membership",
                "Purchase guide",
                "Privacy policy",
                "Terms of service"
            ]
        }
    }
}

</script>



<style scoped lang="scss">
    .section{
        padding: 80px 0;
        background-color: #282935;
    }
    .bg-arrow{
        background-color: #61e6d2;
        width: 50px;
        height: 50px;
    }
    .fixed-bottom {
    position: fixed;
    left: 90vw;
    z-index: 1030;
}
    
</style>