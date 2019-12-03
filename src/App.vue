<template>
  <div id="app">
    <div class="banner">
      <div class="logo">
        <div>Honey</div>
        <div>Lemon</div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'app'
}
</script>

<style scoped lang="scss">
.banner {
  height: 70px;
  background-color: #1c1c1c;
  box-shadow: 5px 5px 5px #888888;

  .logo {
    background-image: url("assets/logo.png");
    background-size: 161px;
    width: 161px;
    height: 124px;
    position: absolute;
    top: 10px;
    left: 50px;
    display: flex;
    flex-direction: column;
    justify-content: center;

    div {
      margin-left: -7px;
      font-weight: bold;
      font-size: 20px;
    }
  }
}
</style>

<style>
html, body {
  margin: 0;
  padding: 0;
}

@font-face {
  font-family: "Eras ITC";
  src: url("assets/Eras ITC Demi.ttf");
}

@font-face {
  font-family: "Eras ITC";
  src: url("assets/Eras ITC Bold.ttf");
  font-weight: bold;
}

#app {
  font-family: 'Eras ITC', 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
