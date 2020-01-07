<template>
  <div class="container">
    <h1>Tebrikler, Halley'i Buldunuz :D</h1>
    <button @click="newGame">Yeni Oyun</button>
  </div>
</template>

<script>
export default {
  methods: {
    newGame() {
      this.$emit("activeComponentEvent", "app-game-cards");
    }
  }
};
</script>

<style scoped>
.container {
  position: absolute;
  top: 0px;
  left: 0px;
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.container h1 {
  text-align: center;
  font-size: 333%;
  color: #8c4c46;
  opacity: 0.5;
}
.container button {
  cursor: pointer;
  width: 200px;
  background-color: #fff;
  color: #af6468;
  border: 1px solid #a0686d;
  height: 50px;
  font-size: 15px;
  border-radius: 5px;
  outline: none;
  transition: all 0.5;
}
.container button :hover {
  background-color: #a0686d;
  color: #fff;
  transition: all 0.5;
}
</style>