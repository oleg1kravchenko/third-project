<template>
    <div>
        <header class="header">
            <div class="container">
                <div class="header__wrapper">
                    <a href="#" class="logo">

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
       phoneMain: "+300000000"
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
    }
    .menu li {
        margin: 0 10px;
    }
    .menu a {
        font-size: 18px;
        font-weight: 700;
        text-transform: uppercase;
        color: #000;
    }
  </style>