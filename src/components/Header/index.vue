<template>
    <b-navbar toggleable="lg" type="dark" variant="dark">
        <b-navbar-brand href="#">NavBar</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
            <b-navbar-nav>
                <b-nav-item v-for="product in products" :href="slug(product.title)" :key="product.id">
                    {{ product.title }}
                </b-nav-item>
            </b-navbar-nav>
        </b-collapse>
    </b-navbar>
</template>

<script>
    export default {
        name: "Header",
        props:{
            products: {
                type: Array,
                required: true
            }
        },
        methods:{
            slug: text => text.split(' ').join('-'),
        }
    }
</script>

<style scoped>

</style>