<template>
  <div class="item" :class="{action:isActive}">
      <slot></slot>
  </div>
</template>

<script>
export default {
    props:{
        isActive:{
            type:Boolean,  //约事该属性的类型是Boolean
            //required:true,  //约束该属性是必须传递
            default:false,  //属性的默认值
        }
    },
}
</script>

<style scoped>
.action{
    background-color: #e7e7e7;
}
.item{
    cursor: pointer;
    width:100%;
    height:100%;
}
.item:hover{
    background-color: #f4f4f4;
}
</style>