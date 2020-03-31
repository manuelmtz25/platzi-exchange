<template>
<div>
    <router-link
      to="/About"
      class="mt-5 text-xl text-green-600 hover:underline"
    >Ir a About</router-link>    
    
    <px-assets-table/>
</div>
    
</template>

<script>
import PxAssetsTable from '@/components/PxAssetsTable'

export default {
    name:"Home",

    components:{PxAssetsTable}
}
</script>