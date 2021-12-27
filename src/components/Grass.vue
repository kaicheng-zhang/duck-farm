<template>
  <div class="land-wrap">
    <div title="水面" class="lake"></div>
    <div title="草" class="grass-1">
      <span></span>
    </div>
    <div title="房子" class="house"></div>
    <div title="树木-1" class="tree-1"></div>
    <div title="树木-2" class="tree-2"></div>
    <!-- 食槽 -->

    <img class="bowl" src="../assets/images/bowl.png" />
  </div>
</template>

<script>
export default {
  name: "",
  data() {
    return {
      tree1: require("../assets/images/tree-1.png"),
    };
  },
  components: {},
  created() {},
  mounted() {},
  methods: {},
};
</script>
<style scoped>
.land-wrap {
  position: absolute;
  width: 100%;
  height: 50%;
  bottom: 0;
  left: 0;
}

.lake {
  width: 100%;
  height: 8rem;
  background: paleturquoise;
  background-image: linear-gradient(180deg, #ebfcff, #65cfdd);
  position: absolute;
  z-index: 1;
  top: -2.5rem;
  filter: blur(1px);
}
.grass-1 {
  position: absolute;
  width: 100%;
  height: 100%;
  bottom: 0;
  left: 0;
  box-shadow: 0 0 5px #fff;
  background-image: linear-gradient(180deg, #b7f03b, #15530b);
  border-top-left-radius: 120% 30%;
  border-top-right-radius: 70% 5%;
  position: relative;
  z-index: 2;
}
.grass-1 span {
  content: "";
  display: block;
  width: 100%;
  height: 80%;
  background-image: linear-gradient(180deg, #b7f03b, #38862c);
  top: 20%;
  border-top-right-radius: 80% 30%;
  opacity: 0.2;
  position: absolute;
  z-index: 2;
}

/*房子*/
.house {
  position: absolute;
  top: -4rem;
  right: -2rem;
  width: 8rem;
  height: 8rem;
  overflow: hidden;
  background: url(../assets/images/house.png) no-repeat;
  z-index: 10;
}

/* 树木 */
.tree-1 {
  position: absolute;
  top: -3rem;
  left: -2rem;
  z-index: 100;
  width: 8rem;
  height: 8rem;
  overflow: hidden;
  background: url(../assets/images/tree-1.png) no-repeat;
  background-size: 100%;
}

.tree-2 {
  position: absolute;
  top: -4rem;
  right: 5rem;
  z-index: 100;
  width: 5rem;
  height: 5rem;
  overflow: hidden;
  background: url(../assets/images/tree-2.png) no-repeat;
  background-size: 100%;
}

.bowl {
  width: 70px;
  height: 30px;
  position: absolute;
  right: 7rem;
  bottom: 5rem;
  z-index: 20;
}
</style>
