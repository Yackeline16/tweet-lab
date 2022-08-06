<template>
  <img v-bind:src="image" className="profile" alt="doggie" />
</template>

<script>
export default {
    name:'ProfileImage',
    props:{
        image:String
    }

}
</script>

<style>

</style>