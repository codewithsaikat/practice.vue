<template>
    <div>
        <ul>
            <li v-for="detail in details" :key="detail.id">{{detail}}</li>
        </ul>
        <br>
        <ul>
            <li v-for="(size, index) in sizes" :key="index">{{size}}</li>
        </ul>
        <br>
        <div v-for="variant in variants" :key="variant.id">{{variant.color}}</div>

    </div>


</template>

<script>
    export default {
        data() {
            return {
                
                details: ['egg', 'milk', 'water', 'sugar'],
                sizes: ['S', 'M', 'L', 'XL'],
                variants: [{
                        id: 2234,
                        color: 'green'
                    },
                    {
                        id: 2235,
                        color: 'blue'
                    }
                ]
            }
        }

    }
</script>
<style scoped>

</style>