<template>
   
    <div v-for="Laptops of laptops.LaptopDetails" :key="Laptops.Brand">

       
        <SingleLaptop :Laptops="Laptops" />

    </div>
    
    
</template>
<script>
import SingleLaptop from "./SingleLaptop.vue"

export default {
    name: 'LaptopList',
    props:{
        laptops: Array
    },
    components: {
        SingleLaptop
    }
    
}
</script>

<style scoped>
.bookbox{

    background-color: bisque;
    padding: 1em;
    color: gray;
    margin: auto;
}
</style>