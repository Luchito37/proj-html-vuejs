<template>
  <div class="sticky-top bg-white">
    <div class="container">
        <nav class="navbar navbar-expand-lg navbar-white bg-white">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">
          <img src="../assets/img/dark-logo.png" alt="" width="" height="24">
        </a>
    <button class="navbar-toggler color-hamburger-menu" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse justify-content-between" id="navbarSupportedContent">
      <ul class=" navbar-nav hamburger-layout">
          <li class="nav-item dropdown" v-for="link in listaLinkHeader" :key="link.name" >
            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              {{link.name}}
            </a>
            <ul class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
              <li><a class="dropdown-item" href="#">{{link.dropdown1}}</a></li>
              <li><a class="dropdown-item" href="#">{{link.dropdown2}}</a></li>
              <li><a class="dropdown-item" href="#">{{link.dropdown3}}</a></li>
            </ul>
          </li>
        </ul>
      <form class="d-flex align-items-center justify-content-center" role="search">
          <div>
              <img :src="require('../assets/img/'+ selectedLeng +'.png')" width="35" height="" alt="">
          </div>
          <select class="border-0 me-2" v-model="selectedLeng" aria-label="Default select example">
              <option selected value="en">ENGLISH</option>
              <option value="fr">FRENCH</option>
              <option value="de">GERMAN</option>
          </select>
          <div class="px-2">
            <i class="fa-solid fa-circle-user"></i>
          </div>
            <input class="border-0" type="" placeholder="Search..." aria-label="Search">
            <button class="btn" type="submit"><i class="fa-solid fa-magnifying-glass"></i></button>
        </form>
    </div>
  </div>
</nav>
    </div>
  </div>
</template>

<script>
export default {
  name: 'TheHeader',
  data(){
    return {
      listaLinkHeader: [
        {
          name: "Home",
          dropdown1: "Build Your Business",
          dropdown2: "Explore How can I help you",
          dropdown3: "Upcoming Events",
        },
        {
          name: "Pages",
          dropdown1: "Build Your Business",
          dropdown2: "Explore How can I help you",
          dropdown3: "You'lI Need a Good Plan",
        },
        {
          name: "Courses",
          dropdown1: "What course i adapt for you?",
          dropdown2: "Help me!",
        },
        {
          name: "Features",
          dropdown1: "Ours stuff",
          dropdown2: "Ours partner",
        },
        {
          name: "Blog",
          dropdown1: "Our Business",
          dropdown2: "News",
          dropdown3: "How you can do it anything",
        },
        {
          name: "Shop",
          dropdown1: "Bought our corses",
          dropdown2: "Explore our price",
        },
      ],
      selectedLeng: "en"
    }
  },

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    .hamburger-layout{
      display: flex;
    flex-direction: row;
    justify-content: space-between;
    }
    .color-hamburger-menu{
      color: #1fad96
    }
</style>
