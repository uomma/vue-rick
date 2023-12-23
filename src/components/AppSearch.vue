<script>
export default {
    name: 'AppSearch'
}
</script>
<template>
    <div class="container">
        <form>
            <div class="row justify-content-center g-1">
                <div class="mb-3 col-12 col-sm-auto ">
                    <label for="search" class="form-label d-none">search</label>
                    <input type="text" class="form-control" id="search" placeholder="Search">
                </div>
                <div class="col-12 col-sm-auto">
                    <label for="search" class="form-label d-none">select status</label>
                    <select class="form-select" id="search">
                        <option selected>Select Status</option>
                        <option value="1">Alive</option>
                        <option value="2">Dead</option>
                        <option value="3">Unknow</option>
                    </select>
                    
                </div>
                <form>
                        <div class="mb-3 col-12 col-sm-auto">
                            <button type="submit" class="btn btn-primary me -1">Submit</button>
                            <button type="reset" class="btn btn-secondary">Reset</button>
                        </div>
                    </form>
            </div>


        </form>
    </div>
</template>



<style lang="scss" scoped></style>