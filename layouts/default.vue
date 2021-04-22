<template>
  <div class="poster">
    <div class="info"></div>
    <div class="picture"></div>
  </div>
</template>

<style>
.poster {
  display: flex;
  justify-content: center;
  position: absolute;
  top: 50%;
  left: 50%;
  margin-right: -50%;
  transform: translate(-50%, -50%);
  width: 1080px;
  height: 1920px;
  background-color: #40362d;
}

.picture {
  margin-right: auto;
  margin-left: auto;
  margin-top: 25px;
  width: 810px;
  height: 1353px;
  background-color: white;
}

.info {
  position: absolute;
  bottom: 0px;
  width: 1080px;
  height: 470px;
  background-color: #2a221b;
}
</style>
