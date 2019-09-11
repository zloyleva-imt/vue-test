<template>
    <div>
        <Header :products="products"/>
        <b-container>
            <b-row class="my-3">
                <ProductCard/>
                <Reviews />
            </b-row>
        </b-container>
    </div>
</template>

<script>
    import Header from './components/Header'
    import ProductCard from './components/ProductCard'
    import Reviews from './components/Reviews'

    export default {
        name: 'App',
        components: {
            Header, ProductCard,Reviews
        },
        data(){
            return {
                products: [
                    {
                        "id": 1,
                        "title": "product with id 1",
                        "img": "img1.png",
                        "text": "lorem ipsum 1"
                    },
                    {
                        "id": 2,
                        "title": "product 2",
                        "img": "img2.png",
                        "text": "lorem ipsum 2"
                    }
                ]
            }
        }
    }
</script>

<style>

</style>
