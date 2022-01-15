<template>
    <div>
        <div>cart({{ cart }})</div>
        <br>
        
        <div>
            <img :src="require(`../assets/images/socks_${img}.jpg`)" >
        </div>
        <div v-for="variant in variants" :key="variant.id" @mouseover="updateImage(variant.color)">{{ variant.color }}</div>
        <br>
        <div>
            <button @click="addToCart">Add to Cart</button>
            <br>
            <br>
            <button @click="removeFromCart">Remove Item</button>
        </div>
        
    </div>

</template>
<script>
    export default {
        data() {
            return {
                cart: 0,
                product: 'Socks',
                img: 'blue',
                inStock: true,
                details: ['50% cotton', '30% wool', '20% polyester'],
                variants: [{
                        id: 2234,
                        color: 'green',
                        // image: './assets/images/socks_green.jpg'
                    },
                    {
                        id: 2235,
                        color: 'blue',
                        // image: './assets/images/socks_blue.jpg'
                    },
                ]

            }
        },
        methods: {
            addToCart() {
                this.cart += 1
            },
            removeFromCart() {
                if (this.cart >= 1) {
                    this.cart -= 1
                }
            },
            updateImage(index){
                this.img = index
            }

        }


    }
</script>