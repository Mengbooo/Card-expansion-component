<script setup>
</script>

<template>
  <div class="symbol" style="display: flex;align-items: center;justify-content:center;position: absolute;top: 10%;transform:translate(-50%,-50%);max-width: 100dvw;background: linear-gradient(217deg, rgba(255,0,0,.8), rgba(255,0,0,0) 70.71%),
            linear-gradient(127deg, rgba(0,255,0,.8), rgba(0,255,0,0) 70.71%),
            linear-gradient(336deg, rgba(0,0,255,.8), rgba(0,0,255,0) 70.71%);
            padding: 20px;border: black 3px solid;border-radius: 15px;">
    <div class="logo">
      <a href="https://github.com/Mengbooo"><img src="./assets/logoooo.jpg" alt=""
          style="width: 50px;border: black 1px solid ; border-radius: 10px;margin-right: 20px;"></a>
    </div>
    <div class="footer">
      <p>Thanks for the inspiration from <a href="https://www.youtube.com/@OnlineTutorialsYT"
          style="color: aqua;text-decoration: none;"><strong>OnlineTutorialsYT</strong></a></p>
      <p>Remastered by <a style="color: aqua;text-decoration: none;"
          href="https://github.com/Mengbooo"><strong>Bolaxious</strong></a></p>
    </div>
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


</template>

<style scoped lang="scss">
.container {
  border: #5e5cfc 3px solid;
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
  transform: rotate(calc(var(--i) * 8deg)) translate(calc(var(--i) * 140px), -100px);
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
