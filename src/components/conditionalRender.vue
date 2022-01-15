<template>
    <div class="product-info">
        <h1>{{ product }}</h1>
        <p v-if="inventory > 10">In stock</p>
        <p v-else-if="inventory <= 10 && inventory > 0">almost sold</p>
        <p v-else> out of stock</p>
        <p v-if="onSale">on Sale!</p>
    </div>
    
</template>
<script>
export default {
    data() {
        return {
            product: 'socks',
            inventory: -1,
            onSale: true

        }
    }
}
</script>