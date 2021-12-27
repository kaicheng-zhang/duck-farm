<template>
  <div title="白云" class="clouds">
    <div class="cloud x1"></div>
    <div class="cloud x2"></div>
    <div class="cloud x3"></div>
  </div>
</template>

<script>
export default {};
</script>
<style scoped>
/*白云*/

.cloud {
  position: absolute;
  top: 2rem;
  width: 5rem;
  height: 2.5rem;
  border-radius: 3rem;
  background-color: #cfeffd;
  filter: blur(5px);
}

.cloud:before {
  content: "";
  position: absolute;
  background: #cfeffd;
  width: 5rem;
  height: 0.8rem;
  border-radius: 0.5rem;
  bottom: 0;
}

.cloud.x1 {
  left: -30%;
  -webkit-animation: cloud 80s linear infinite;
}

.cloud.x1:before {
  left: -1rem;
}

.cloud.x2 {
  right: -30%;
  top: 8rem;
  width: 4rem;
  height: 1.6rem;
  -webkit-animation: cloudx2 150s linear infinite;
}

.cloud.x2:before {
  width: 3rem;
  height: 0.6rem;
  right: 1.8rem;
}

.cloud.x3 {
  left: -50%;
  top: 12.5rem;
  width: 3rem;
  height: 1.4rem;
  -webkit-animation: cloudx3 120s linear infinite;
}

.cloud.x3:before {
  width: 2rem;
  height: 0.4rem;
  left: 1.8rem;
}



@-webkit-keyframes cloud {
  0% {
    left: -30%;
  }

  50% {
    left: 120%;
  }

  100% {
    left: -30%;
  }
}

@-webkit-keyframes cloudx2 {
  0% {
    right: -30%;
  }

  50% {
    right: 130%;
  }

  100% {
    right: -30%;
  }
}

@-webkit-keyframes cloudx3 {
  0% {
    left: -50%;
  }

  50% {
    left: 150%;
  }

  100% {
    left: -50%;
  }
}
</style>
