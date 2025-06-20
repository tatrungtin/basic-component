<template>
  <section class="container">
    <div class="row">
        <div class="col-sm-3">
            <ProductItem 
                urlImage="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ1zwhySGCEBxRRFYIcQgvOLOpRGqrT3d7Qng&s"
                nameProduct="Hinh 1"
                proItem = '{
                    urlImage :"sds",
                    nameProduct :"Macbook"
                }'
            />
        </div>
        <div class="col-sm-3">
            <ProductItem
                urlImage="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ1zwhySGCEBxRRFYIcQgvOLOpRGqrT3d7Qng&s"
                nameProduct="Hinh 2"
            />
        </div>
        <div class="col-sm-3">
            <ProductItem
            urlImage="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ1zwhySGCEBxRRFYIcQgvOLOpRGqrT3d7Qng&s"
                nameProduct="Hinh 3"
            />
        </div>
        <div class="col-sm-3">
            <ProductItem
                urlImage="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ1zwhySGCEBxRRFYIcQgvOLOpRGqrT3d7Qng&s"
                nameProduct="Hinh 4"
            />
        </div>
    </div>
  </section>
</template>

<script>
import ProductItem from './ProductItem.vue';
export default {
    components: {
        ProductItem
    }
}
</script>

<style>

</style>