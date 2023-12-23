<script>
import AppCard from './AppCard.vue';
export default {
    name: 'AppList',
    components:{
        AppCard
    }
}
</script>

<template>
    <div class="container">
        <div class="row">
            <div class="col-12 col-sm-4">
                <AppCard></AppCard>
            </div>
        </div>
    </div>
</template>



<style lang="scss" scoped></style>