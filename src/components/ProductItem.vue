<template>
   <div class="card text-left">
        <img class="card-img-top" :src="urlImage">
        <div class="card-body">
            <h4 class="card-title">{{ proItem.nameProduct}}</h4>
            <p class="card-text">Conten 1</p>
        </div>
    </div>
</template>

<script>
export default {
    props:{
        urlImage :{
            type : String
        },
        nameProduct: {
            type : String
        },
        proItem :{
            Object
        }
    }
}
</script>

<style>

</style>