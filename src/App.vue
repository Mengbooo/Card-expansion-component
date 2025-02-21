<script setup>
</script>

<template>
  <div style="position: absolute;top: 30px;transform: translateX(-50%);user-select: none;">
    <a href="https://github.com/Mengbooo"><img src="./assets/logoooo.jpg" alt=""
        style="width: 50px; border-radius: 10px;"></a>
  </div>

  <div class="container">
    <div class="card" style="--i: -4;">Wh</div>
    <div class="card" style="--i: -3;">at</div>
    <div class="card" style="--i: -2;">can</div>
    <div class="card" style="--i: -1;">I</div>
    <div class="card" style="--i: -0;">say</div>
    <div class="card" style="--i: 1;">man</div>
    <div class="card" style="--i: 2;">ba</div>
    <div class="card" style="--i: 3;">out</div>
    <div class="card" style="--i: 4;">!</div>
  </div>
  <div style="user-select: none;position: absolute;bottom: 20px;transform: translateX(-50%);color: white;z-index: 999;">
    <p>Thanks for the inspiration from <a href="https://www.youtube.com/@OnlineTutorialsYT"
        style="color: aqua;text-decoration: none;"><strong>OnlineTutorialsYT</strong></a></p>
    <p>Remastered by <a style="color: aqua;text-decoration: none;"
        href="https://github.com/Mengbooo"><strong>Bolaxious</strong></a></p>
  </div>

</template>

<style lang="scss">
@font-face {
  font-family: 'Ubuntu';
  src: url('../font/Ubuntu-Bold.ttf');
  font-weight: normal;
  font-style: normal;
};

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Ubuntu", sans-serif;
}

body {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  background-color: #0f0f0f;
}

.container {
  width: 100%;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
}

.container .card {
  position: absolute;
  width: 350px;
  height: 520px;
  background-color: #5e5cfc;
  color: rgba(0, 0, 0, 0);
  display: flex;
  justify-content: center;
  align-items: center;
  color: rgba(0, 0, 0, 0);
  font-size: 8em;
  font-weight: 700;
  border: 10px solid rgba(0, 0, 0, 0.1);
  border-radius: 20px;
  cursor: pointer;
  transition: 0.52s;
  transform-origin: 50% 100%;
  filter: hue-rotate(calc(var(--i) * 30deg));
  box-shadow: 0 15px 50px rgba(0, 0, 0, 0.1);
  user-select: none;
  -webkit-user-select: none;
}

.container:hover .card {
  transform: rotate(calc(var(--i) * 8deg))
    translate(calc(var(--i) * 140px), -100px);
  color: rgba(0, 0, 0, 0.25);
  box-shadow: 0 15px 50px rgba(0, 0, 0, 0.25);
}

.container:active .card {
  background-color: #333;
}

.container .card:active {
  translate: calc(var(--i) * 20px) -50px;
  z-index: 1;
  background-color: #5e5cfc;
}

</style>
