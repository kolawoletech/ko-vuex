<template>
    <div id="product-list-one">
        <h2>Product List One</h2>
        <ul>
            <li v-for="product in products">
                <span class="name">{{ product.name }}</span>
                <span class="name">{{ product.price }}</span>
            </li>
        </ul>
    </div>
</template>
<script>
export default {
    name: "ProductList",
    props: ['products'],
    data() {
        return {

        }
    }
}
</script>