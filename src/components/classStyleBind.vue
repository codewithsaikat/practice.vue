<template>
    <div>
        <div>cart({{ cart }})</div>
        <br>
        <div>
            <p v-if="inStock">In Stock</p>
            <p v-else> Out of Stock</p>
        </div>
        <div>
            <img :class="{ 'out-of-stock-img': !inStock }" :src="require(`../assets/images/socks_${img}.jpg`)">
        </div>
        <div v-for="variant in variants" :key="variant.id" @mouseover="updateImage(variant.color)"
            :style="{ backgroundColor: variant.color}">{{ variant.color }}
        </div>
        <br>

        <div>
            <button :class="{disabledButton: !inStock}" :disable="!inStock" @click="addToCart">Add to Cart</button>
            <br>
            <br>

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
                inStock: false,
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
            updateImage(index) {
                this.img = index
            }

        }


    }
</script>