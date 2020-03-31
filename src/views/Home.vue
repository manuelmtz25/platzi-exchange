<template>
  <div>
    <router-link to="/About" class="mt-5 text-xl text-green-600 hover:underline"
      >Ir a About</router-link
    >

    <px-assets-table :assets="assets"/>
  </div>
</template>

<script>
import api from '@/api'
import PxAssetsTable from "@/components/PxAssetsTable";

export default {
  name: "Home",

  components: { PxAssetsTable },

  data(){
      return{
          assets:[]
      }
  },

  created(){
      api.getAssets().then(assets=>(this.assets=assets))
  }
};
</script>
