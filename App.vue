
<template>
  <Home v-if="!$route.path" /> <router-view v-else /> </template>

<script>
import { RouterView } from 'vue-router'; // Import only necessary component
import Home from './views/HomeView.vue';
import store from './store.js';

export default {
  components: {
    Home, // Locally register Home component
    RouterView
  },
  data() {
    return {
      store
    };
  },
  mounted() {
    fetch(this.store.api)
      .then(res => res.json())
      .then(res => {
        console.log(res);
        this.store.database = res;
        this.store.spiner = false;
      })
      .catch(err => {
        console.log(err);
        this.store.spiner = false;
      });
  }
};
</script>




<!-- <template>
  <div v-if="!$route.path">
      <Home />
    </div>

    Route content 
    <router-view v-if="$route.path"></router-view>
</template>

<script>
import { RouterLink, RouterView } from 'vue-router'
import Home from './views/HomeView.vue'
import store from './store.js'

export default{
  data(){
    return{
      store
    }
  },
  mounted(){
    fetch(this.store.api).then(res => res.json()).then(res=>{
      console.log(res)
      this.store.database = res
      this.store.spiner = false
    }).catch(err => {
      console.log(err)
      this.store.spiner = false
    })
  }
}
</script> -->