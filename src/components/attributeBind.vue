<template>
<div id= "app">
    <h1>{{product}}</h1>
    <div>
        <img :src="require(`../assets/images/socks_blue.jpg`)" />
    </div>
    <a :href="url">Vue Mastery</a>
</div>
    
</template>
<script>

export default {
    
    data(){
        return{
            product: 'Socks',
            image:'socks_blue.jpg',
            url: 'https://www.vuemastery.com/'
        }
    }
    
}
</script>





    
