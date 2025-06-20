<template>
  <section class="container">
    <div class="row">
        <div class="col-sm-3" v-for="(proItem, index) in proList" :key="index">
            <ProductItem 
                :proItem= "proItem"
                 multipleType="Tin ta"
                 @custom-handle-select="handleSelect(proItem)"
            />
        </div>
    </div>
  </section>
</template>

<script>
import ProductItem from './ProductItem.vue';
export default {
    methods :{
        handleSelect(proItem){
            console.log('da nhan', proItem)
        }
    },  
    data(){
        return {
            proList :[
            {
                urlImage :"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ1zwhySGCEBxRRFYIcQgvOLOpRGqrT3d7Qng&s",
                nameProduct :"Macbook"
            },
            {
                urlImage :"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ1zwhySGCEBxRRFYIcQgvOLOpRGqrT3d7Qng&s",
                nameProduct :"Macbook air"
            },
            {
                urlImage :"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ1zwhySGCEBxRRFYIcQgvOLOpRGqrT3d7Qng&s",
                nameProduct :"Macbook pro"
            },
            {
                urlImage :"https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ1zwhySGCEBxRRFYIcQgvOLOpRGqrT3d7Qng&s",
                nameProduct :"Macbook"
            }
            ]
           
        }
    },
    components: {
        ProductItem
    },
    mounted: function () {
        console.log('product list')
    }
}
</script>

<style>

</style>