<template>
  <section class="welcome-screen">
    <div class="window blur">
      <h1 class="main-title">Добро пожаловать в Olivence</h1>
      <h2>Пример х2</h2>
      <h3>Пример х3</h3>
      <h4>Пример х4</h4>
      <h5>Пример х5</h5>
      <h6>Пример х6</h6>
      <p>Welcome to Olivence</p>
      <a>Добро пожаловать в Olivence</a>
      <button class="enter-btn">
        идти
        <span>идти</span>
        <span>идти</span>
        <span>в меню</span>
      </button>
    </div>
  </section>
</template>

<script>
export default {
  name: "WelcomeScreen",
};
</script>

<style>
.welcome-screen {
  text-align: center;
  background-image: url("/assets/css/img/bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  justify-content: center;
}
.window {
  max-height: max-content;
  max-width: max-content;
  padding: 40px;
  margin: 50px;
  overflow: hidden;
  border-radius: 10px;
  background-color: var(--oliv-fade02);
}
.blur {
  backdrop-filter: blur(10px);
  background-size: cover;
  box-shadow: rgba(0, 0, 0, 0.56) 0px 22px 70px 4px;
  border: 1px solid var(--oliv-light02);
}
button {

  box-shadow: rgba(0, 0, 0, 0.17) 0px -23px 25px 0px inset,
    rgba(0, 0, 0, 0.15) 0px -36px 30px 0px inset,
    rgba(0, 0, 0, 0.1) 0px -79px 40px 0px inset, rgba(0, 0, 0, 0.06) 0px 2px 1px,
    rgba(0, 0, 0, 0.09) 0px 4px 2px, rgba(0, 0, 0, 0.09) 0px 8px 4px,
    rgba(0, 0, 0, 0.09) 0px 16px 8px, rgba(0, 0, 0, 0.09) 0px 32px 16px;
}
.enter-btn {
  margin: 0;
  padding: 0;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 6em;
  color: transparent;
  text-transform: uppercase;
}
.enter-btn span:nth-child(1) {
  position: absolute;
  top: 0;
  left: 0;
  color: #000;
  transition: 0.5s;
  clip-path: polygon(0 0, 100% 0, 100% 50%, 0 50%);
  overflow: hidden;
}
.enter-btn:hover span:nth-child(1) {
  transform: translateY(-18px);
}
.enter-btn span:nth-child(2) {
  position: absolute;
  top: 0;
  left: 0;
  color: #000;
  transition: 0.5s;
  clip-path: polygon(0 50%, 100% 50%, 100% 100%, 0 100%);
  overflow: hidden;
}
.enter-btn:hover span:nth-child(2) {
  transform: translateY(18px);
}
.enter-btn span:nth-child(3) {
  position: absolute;
  top: 50%;
  left: 0;
  transform: translateY(-50%) scaleY(0);
  width: 91%;
  color: #000;
  background: #ff0;
  font-size: 0.25em;
  font-weight: 500;
  letter-spacing: 0.7em;
  text-align: center;
  padding-left: 20px;
  margin-left: 5px;
  transition: 0.5s;
}
.enter-btn:hover span:nth-child(3) {
  transform: translateY(-50%) scaleY(1);
}
</style>
