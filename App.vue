<template>
  <view class="container">
    <status-bar background-color="black" bar-style="light-content" />
    <text class="text-login">Login</text>
    <text class="label">E-mail</text>
    <text-input class="input"/>
    <text class="label">Senha</text>
    <text-input class="input"/>
    <view class="itens"> 
      <text class="recuperar">Esqueceu a senha?</text>
      <button class="btn-entrar" title="Login" color="black" :on-press="pressionar"></button>
    </view>

  </view>
</template>

<script>
export default {
  data() {
    return {
      email: "E-mail",
      senha: "Senha",
    };
  },
  methods: {
    pressionar: function () {
      alert("Olá, usuário! Você está na tela de Login.");
    },
  },
};
</script>

<style>
.container {
  background-color: white;
  align-items: center;
  display: flex;
}

.itens {
  display: flex;
}

.recuperar {
  align-self: flex-start;
  margin: 15px 10px;
}

.label {
  align-self: flex-start;
}
.text-login {
  margin: 20%;
  font-size: 40px;
  color: black;
}

.input {
  width: 98%;
  margin: 10px 10px;
  border-radius: 1px;
  padding: 10px;
  border-width: 1;
}
</style>
