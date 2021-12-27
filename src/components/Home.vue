<template>
  <div class="home">
    <User />
    <div>
      <Sunlight />
      <Cloud />
      <GrassLand />
      <Chick />
      <Egg/>
    </div>
    <Nav />
    <PopMask />
  </div>
</template>

<script>
import User from "./User.vue";
import Nav from "./Nav.vue";
// 阳光
import Sunlight from "./Sunlight.vue";

// 云朵
import Cloud from "./Cloud.vue";
// 草地
import GrassLand from "./Grass.vue";

// 小鸡
import Chick from "./Chick.vue";

// poplayer
import PopMask from "./PopMask.vue";

// 鸡蛋
import Egg from './Egg.vue'

export default {
  name: "home",
  components: {
    User,
    Nav,
    Sunlight,
    Cloud,
    GrassLand,
    Chick,
    PopMask,
    Egg
  },
  setup(props, ctx) {
    const openDraw = () => {
      console.log("open ...");
    };
    return {
      openDraw,
    };
  },
};
</script>
<style scoped lang="scss">
.home {
  width: 100%;
  height: 100%;
  position: absolute;
  bottom: 0;
  background-image: -webkit-linear-gradient(to bottom, #4aaeff, #fff);
  background-image: linear-gradient(to bottom, #4aaeff, #fff);
  overflow: hidden;
}
</style>
