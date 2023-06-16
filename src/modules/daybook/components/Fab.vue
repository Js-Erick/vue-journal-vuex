<template>
  <div>
    <button class="btn btn-primary">
       <i class="fa fa-2x"
       :class="icon"></i>
          
    </button>
  </div>
</template>
<script>
export default {
  props:{
    icon:{
      type:String,
      default:'fa-plus'
    }
  }
}
</script>

<style lang="scss" scoped>
button {
    position:fixed;
    bottom:30px;
    right:50px;
    width:70px;
    height:70px;
    border-radius: 80%;
}
</style>