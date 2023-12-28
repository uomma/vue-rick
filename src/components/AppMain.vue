<script>
import AppSearch from './AppSearch.vue';
import AppList from './AppList.vue';
export default {
   name:'AppMain',
   components:{
    AppSearch,
    AppList
   },
   methods:{
    handleSearch(){
        console.log('ho csca');
        this.$emit('algo')
      
    }
   }
}
</script>
<template>
    <AppSearch @search="handleSearch"/>
    <AppList></AppList>
  
</template>



<style lang="scss" scoped></style>