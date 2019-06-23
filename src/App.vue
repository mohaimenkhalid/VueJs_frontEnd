<template>
  <div class="wrapper">
    <div class="header">
            <div class="logo"></div>
            <div class="logo1"><font size="6.5">ECONFIRM</font><br/>
            <font size="1">OUR BUSSINESS IS RENEWABLE</font>
            
            </div>
             <div class="information">
               Contact Us: 1-800-555-1214<br/>
               Fax: 1-800-555-1417<br/>
               Email: info@ecofarm.com
             </div>
            <div class="nav">
              <ul>
              <li><router-link to="/" exact>Home</router-link></li>
              <li><router-link to="/about">About US</router-link></li>
              <li><router-link to="/service">Services</router-link></li>
              <!-- <li><router-link to="">Stratagy</router-link></li>
              <li><router-link to="">Product</router-link></li>
              <li><router-link to="">Resorces</router-link></li>
              <li><router-link to="">Contacts</router-link></li> -->
              
          </ul>
            </div>
       </div>
       
       <router-view></router-view>
       
          
       <div class="footer">
          <pre>@2006-2014khalid.All Rights Reserved   <a href="sitemap.html">Sitemap</a> <a href="productaa.html">Products</a> <a href="bussiness.html">Bussiness</a> <a href="contactss.html">Contact</a> <a href="partnar.html">Partnar</a> <a href="home22.html">Home</a> </pre>
         
       </div>
  </div>
</template>

<script>
import VueRouter from 'vue-router'
import Home from './pages/Home.vue'
import About from './pages/About.vue'
import Service from './pages/Service.vue'

const routes = [
  { path: '/', component: Home },
  { path: '/about', component: About },
  { path: '/service', component: Service }
 
]


const router = new VueRouter({
  routes : routes, // short for `routes: routes` or routes
  mode: 'history'
})




export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },

  router : router

}
</script>

