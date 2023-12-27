<script>
import AppCard from './AppCard.vue';
import { store } from '../store';
export default {
    name: 'AppList',
    components:{
        AppCard
    },
    data(){
        return{
            store,
            characters:[],
        }
    },

}
</script> 

<template>
    <div class="container">
        <div class="row">
            <div class="col-12 col-sm-3"  v-for="character in store.characters">
                <AppCard :img="character.image" :title="character.name" :status="character.status" :species="character.species"/>
            </div>
        </div>
    </div>
</template>



<style lang="scss" scoped></style>