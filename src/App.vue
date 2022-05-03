<template>
  <div id="home">
    <div class="my center">
      app
    </div>
    <div class=""></div>
  </div>
</template>

<script>
import { ref } from "vue";
export default {
  name: "App",
  setup() {
    let me = ref([5, 5, 5, 4, 3, 2, 2]);
    console.log(me);
    function changeme() {
      me.value.push(100);
      console.log(me);
    }
    return {
      me,
      changeme,
    };
  },
};
</script>

<style lang='less'>
#app {
  
    width: 100%;
    height: 100%;
  #home {
    width: 100%;
    height: 100%;
    background-color: antiquewhite;
  }
}
</style>
