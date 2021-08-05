<template>
  <div class="w-96 min-h-screen flex items-center">
    <div class="relative turntable border-none border-red-500 left-1/2">
      <div class="piece border-none border-red-500 absolute top-0"></div>
      <div class="piece border-none border-red-500 absolute top-0 rotate30"></div>
      <div class="piece border-none border-red-500 absolute top-0 rotate60"></div>
      <div class="piece border-none border-red-500 absolute top-0 rotate90"></div>
      <div class="piece border-none border-red-500 absolute top-0 rotate120"></div>
      <div class="piece border-none border-red-500 absolute top-0 rotate150"></div>
      <div class="piece border-none border-red-500 absolute top-0 rotate180"></div>
      <div class="piece border-none border-red-500 absolute top-0 rotate210"></div>
      <div class="piece border-none border-red-500 absolute top-0 rotate240"></div>
      <div class="piece border-none border-red-500 absolute top-0 rotate270"></div>
      <div class="piece border-none border-red-500 absolute top-0 rotate300"></div>
      <div class="piece border-none border-red-500 absolute top-0 rotate330"></div>
      <div class="piece border-none border-red-500 absolute top-0 rotate360"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Turntable',
  layout: 'MobileLayout'
};
</script>

<style scoped lang="scss">
.piece {
  width: 150px;
  height: 300px;
    //background-color #f6d365
    //border-bottom-right-radius 150px
  border-top-right-radius: 150px;
}
.turntable {
  width: 150px;
  height: 300px;
  transform-origin: left center;
  animation: myRotate infinite 4s ease-in-out;
  div {
    transform-origin: left center;
  }
  .rotate30 {
    transform: rotate(30deg);
    background-image: linear-gradient(120deg, #f6d365, #f6d365 75px, transparent 75px);
  }
  .rotate60 {
    transform: rotate(60deg);
    background-image: linear-gradient(120deg, red, red 75px, transparent 75px);
  }
  .rotate90 {
    transform: rotate(90deg);
    background-image: linear-gradient(120deg, green, green 75px, transparent 75px);
  }
  .rotate120 {
    transform: rotate(120deg);
    background-image: linear-gradient(120deg, blue, blue 75px, transparent 75px);
  }
  .rotate150 {
    transform: rotate(150deg);
    background-image: linear-gradient(120deg, #f68865, #f68865 75px, transparent 75px);
  }
  .rotate180 {
    transform: rotate(180deg);
    background-image: linear-gradient(120deg, #f66665, #f66665 75px, transparent 75px);
  }
  .rotate210 {
    transform: rotate(210deg);
    background-image: linear-gradient(120deg, #f22222, #f22222 75px, transparent 75px);
  }
  .rotate240 {
    transform: rotate(240deg);
    background-image: linear-gradient(120deg, #d6d365, #d6d365 75px, transparent 75px);
  }
  .rotate240 {
    transform: rotate(240deg);
    background-image: linear-gradient(120deg, skyblue, skyblue 75px, transparent 75px);
  }
  .rotate270 {
    transform: rotate(270deg);
    background-image: linear-gradient(120deg, pink, pink 75px, transparent 75px);
  }
  .rotate300 {
    transform: rotate(300deg);
    background-image: linear-gradient(120deg, gray, gray 75px, transparent 75px);
  }
  .rotate330 {
    transform: rotate(330deg);
    background-image: linear-gradient(120deg, yellowgreen, yellowgreen 75px, transparent 75px);
  }
  .rotate360 {
    transform: rotate(360deg);
    background-image: linear-gradient(120deg, black, black 75px, transparent 75px);
  }

}

@keyframes myRotate {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(720deg);
  }
}
</style>
