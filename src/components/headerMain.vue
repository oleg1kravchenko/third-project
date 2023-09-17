<template>
    <div>
        <header class="header">
            <div class="container">
                <div class="header__wrapper">
                    <a href="#" class="logo">
                    <img :src="logo" alt="alt">
                    </a>
                    <ul class="menu">
                        <li v-for="itemMenu in menu"><a :href="itemMenu.href">{{ itemMenu.title }}</a></li>
                    </ul>
                    <a :href="phoneMain" class="phone-main">{{ phoneMain }}</a>
                </div>
            </div>
        </header>
    </div>
  </template>
  
  <script>
  export default {
    name: 'headerMain',
    data () {
      return {
       menu: [
        {title: "About", href: "/about"},
        {title: "Catalog", href: "/catalog"},
        {title: "Team", href: "/team"},
        {title: "Contacts", href: "/contacts"},
       ],
       phoneMain: "+300000000",
       logo: require('../assets/logo.png'),
      }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
    .menu {
        display: flex;
        align-items: center;
        justify-content: center;
        background-image: url(../assets/partner5.png);
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
    }
    .menu li {
        margin: 0 14px;
    }
    .menu a {
        font-size: 18px;
        font-weight: 700;
        text-transform: uppercase;
        color: #000;
    }
    .header {
        background-image: url('../assets/news1.jpg');
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
    }
  </style>