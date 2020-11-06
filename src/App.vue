<template>
  <div>
    <h1>第一个VUE工程</h1>
    <div style="height:70px;">
    <Item :isActive="curActive === 'a1'" @active="curActive = 'a1'">
      <h4>我的第一个组件</h4>
    </Item>
    </div>
    <div style="height:70px;">
    <Item :isActive="curActive === 'a2'" @active="curActive = 'a2'">
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
  },
  data(){
    return {
      curActive:'a1',
    }
  },
  methods:{
    test(e){
      console.log(e);
    }
  }
}
</script>