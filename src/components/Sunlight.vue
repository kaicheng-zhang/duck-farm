<template>
  <div class="sunlight">
    <span></span> <span></span> <span></span> <span></span>
  </div>
</template>

<script>
export default {
  name: "sunlight"
};
</script>
<style scoped>
/*太阳光 sunlight*/
.sunlight {
  position: absolute;
  width: 100%;
  height: 100%;
  overflow: hidden;
}

.sunlight span {
  position: absolute;
  top: -10%;
  height: 150%;
  width: 3rem;
  background-color: #fff;
  left: 20%;
  transform: rotate(-14deg);
  z-index: 20;
}

.sunlight span:nth-child(1) {
  -webkit-animation: sunlight-1 11s ease-in infinite;
}

.sunlight span:nth-child(2) {
  left: 28%;
  -webkit-animation: sunlight-2 11.5s ease-in infinite;
}

.sunlight span:nth-child(3) {
  left: 65%;
  width: 5rem;
  transform: rotate(-18deg);
  -webkit-animation: sunlight-3 13s ease-in infinite;
}

.sunlight span:nth-child(4) {
  left: 108%;
  width: 1.6rem;
  transform: rotate(-22deg);
  -webkit-animation: sunlight-3 15s ease-in infinite;
}

@-webkit-keyframes sunlight-1 {
  0% {
    opacity: 0;
  }

  50% {
    opacity: 0.15;
  }

  100% {
    opacity: 0;
  }
}

@-webkit-keyframes sunlight-2 {
  0% {
    opacity: 0;
  }

  50% {
    opacity: 0.1;
  }

  100% {
    opacity: 0;
  }
}

@-webkit-keyframes sunlight-3 {
  0% {
    opacity: 0;
  }

  50% {
    opacity: 0.08;
  }

  100% {
    opacity: 0;
  }
}
</style>
