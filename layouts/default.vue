<template>
  <div class="poster">
    <div class="info">
    </div>
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
  width: 541px;
  height: 900px;
  background-color: #40362d;
}

.picture {
  margin-top: 15px;
  width: 368px;
  height: 658px;
  background-color: white;
}

.info {
  position: absolute;
  bottom: 0px;
  width: 541px;
  height: 217px;
  background-color: #2a221b;
}
</style>
