<template>
   <div class="card text-left">
        <img class="card-img-top" :src="proItem.urlImage">
        <div class="card-body">
            <h4 class="card-title">{{ proItem.nameProduct }}</h4>
            <p class="card-text">{{ proItem.nameProduct }}</p>
            <button class="btn btn-info"
                @click="handleSelect(proItem)"
            >Chọn</button>
            <p>{{ user }}</p>
        </div>
    </div>
</template>

<script>
export default {
    props:{
        proItem :{
            type :Object,
            default: () => ({}),
            required :true
        },
        multipleType:{
            type :[String, Number],
            default :"hello",
            validator(value){
                if(value.length > 3){
                    return true;
                }else{
                    return false;
                }
            },

        }
    },
    mounted: function () {
        // console.log(this.proItem)
    },
    methods :{
        handleSelect(proItem){
            this.$emit("customHandleSelect", proItem)
        }
    },
    inject :["user"]

}
</script>

<style>

</style>