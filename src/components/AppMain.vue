<script>
import AppSearch from './AppSearch.vue';
import AppList from './AppList.vue';
export default {
   name:'AppMain',
   components:{
    AppSearch,
    AppList
   }
}
</script>
<template>
    <AppSearch> </AppSearch>
    <AppList></AppList>
  
</template>



<style lang="scss" scoped></style>