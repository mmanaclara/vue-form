<script setup>
function logout() {
  console.log("Logout")
}
</script>

<template>
  <div class="container">
    <h2>Boas-vindas, Nome!</h2>
    <strong>Aproveite todos os nossos serviços!</strong> <br />
      <a href="/">Sair</a>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  padding-right: 10rem;
}

a {
  width: fit-content;
  padding: 0.4rem 0.8rem;
  border: 1px solid hsla(160, 100%, 37%, 1);
  border-radius: 8px;
}
</style>
