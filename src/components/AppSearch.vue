<script>
import { store } from '../store';
export default {
    name: 'AppSearch',
    data() {
        return {
            store
        }
    },
    methods: {
       /*  testSubmit() {
            console.log(this.store.searchKey)
        } */
    }
}
</script>
<template>
    <div class="container">
        <form @submit.prevent="$emit('search')">
            <div class="row justify-content-center g-1">
                <div class="mb-3 col-12 col-sm-auto ">
                    <label for="search" class="form-label d-none">search</label>
                    <input type="text" class="form-control" id="search" placeholder="Search" v-model="store.searchKey">
                </div>
                <div class="col-12 col-sm-auto">
                    <label for="search" class="form-label d-none">select status</label>
                    <select class="form-select" id="search" v-model="store.searchStatus">
                        <option selected value="">Select Status</option>
                        <option value="Alive">Alive</option>
                        <option value="Dead">Dead</option>
                        <option value="Unknow">Unknow</option>
                    </select>

                </div>
                
                    <div class="mb-3 col-12 col-sm-auto">
                        <button type="submit" class="btn btn-primary me -1">Submit</button>
                        <button type="reset" class="btn btn-secondary">Reset</button>
                    </div>
                
            </div>


        </form>
    </div>
</template>



<style lang="scss" scoped></style>