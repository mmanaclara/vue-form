<script setup>
import { RouterLink } from 'vue-router'
function login() {
  console.log("Login")
}
</script>

<template>
  <main>
    <h2>Login</h2>

    <form @submit.prevent="login">
      <label>
        E-mail
        <input type="text" placeholder="Digite seu e-mail" v-model="email" />
      </label>

      <label>
        Senha
        <input type="password" placeholder="Digite sua senha" v-model="password" />
      </label>

      <button type="submit">
        <RouterLink to="/login">Enviar</RouterLink>
      </button>
    </form>
  </main>
</template>

<style scoped>
main {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 1.6rem;
  width: 100%;
  padding-right: 6rem;
}

form {
  display: flex;
  flex-direction: column;
  gap: 1.2rem;
  width: 20rem;
}

label {
  display: flex;
  flex-direction: column;
  gap: 0.2rem;
}

input {
  padding: 0.5rem;
  border-radius: 8px;
  border: none;
  outline: 0;
}

button {
  background: transparent;
  border: none;
  line-height: 0;
  align-self: center;
}

a {
  margin-top: 1rem;
  padding: 0.6rem;
  border-radius: 8px;
  text-transform: uppercase;
  background: hsla(160, 100%, 37%, 1);
  border: 0;
  color: black;
  font-weight: bold;
  width: 20rem;
  height: 2.4rem;
  
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
