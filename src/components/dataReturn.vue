<template>
<div>
     <h1>{{product}}</h1>
     <h2>{{value}}</h2>
    
</div>   
</template>
<script>
export default {
    props: {
        value: String
    },
    data(){
        return {
            product: 'cup',
            
        }
    }
}
</script>