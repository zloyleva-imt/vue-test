<template>
    <b-col md="6">
        <h1 class="text-capitalize border-bottom">{{ product.title }}</h1>
        <div class="my-4"><img :src="imgLink" class="rounded">
        </div>
        <div class="border-top"><h3 class="h4">Product description</h3>
            <p>{{ product.text }}</p>
        </div>
    </b-col>
</template>

<script>
    export default {
        name: "ProductCard",
        props:{
            product:{
                type: Object,
                required:true
            }
        },
        computed:{
            imgLink(){
                return `http://smktesting.herokuapp.com/static/${this.product.img}`
            }
        }
    }
</script>

<style scoped>

</style>