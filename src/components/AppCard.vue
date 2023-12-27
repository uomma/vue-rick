<script>
export default {
    name: 'AppCard',
    props:{
        img: String,
        title: String,
        status: String,
        species: String
    }
}
</script>

<template>
    <div class="text-center">
        <div class="img"><img class="rounded-circle image-fluid" :src="img" alt=""></div>
        <h3>{{ title }}</h3>
        <div>{{status}}</div>
        <div>{{species}}</div>
    </div>
</template>



<style lang="scss" scoped></style>