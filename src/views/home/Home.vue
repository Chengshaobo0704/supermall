<template>
  <div></div>
</template>

<script>
    import {getHomeMultidata} from '../../network/home'
  

  export default {
    name: "Home",
    components: {
     
    },
    data() {
      return {
         banners:[],
         recommends:[],
      }
    },
    created() {
      this.getHomeMultidata()
    },
    methods: {
      getHomeMultidata(){
        getHomeMultidata().then(res => {
         this.banners = res.data.banner.list;
         this.recommends = res.data.recommend.list;
         console.log(res);
      })
      }
    },
    computed: {
    
    },
  }
</script>

<style>
  
</style>
