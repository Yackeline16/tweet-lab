<template>
  <p className="message">
        {{ msg }}
   </p>
</template>

<script>
export default {
    name:'Message',
    props:{
        msg:String
    }

}
</script>

<style>

</style>