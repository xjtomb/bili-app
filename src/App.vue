<template>
  <div>
    <h1>第一个VUE工程</h1>
    <div style="height:70px;">
    <Item>
      <h4>我的第一个组件</h4>
    </Item>
    </div>

  </div>
</template>

<script>
import Item from "./components/Item"
export default {
  components:{
    Item
  }
}
</script>