<template>
 <div class="col-md-6">
     <img v-bind:src="oneroom.image" alt="" width="100%">
     <h4>{{oneroom.title}}</h4>
    <p>{{oneroom.price}}원</p>
 </div>
</template>

<script>
export default {
    name : "card",
    props : {
        oneroom : Object
    }
}
</script>

<style>

</style>
