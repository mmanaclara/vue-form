<script setup>
import { RouterLink } from 'vue-router'
import { reactive, onMounted } from 'vue'

// onMounted(() => {
//   const companyServices = reactive([
//     {
//       id: 1,
//       title: 'Mudança residencial',
//       description: 'Estamos preparados para fazer mudanças residenciais de casas ou apartamentos com eficiência e qualidade.'
//     },
//     {
//       id: 2,
//       title: 'Mudança comercial',
//       description: 'Eficiente e discreto, esse é o serviço que buscamos oferecer para nossos clientes que desejam transportar mudanças comerciais.'
//     },
//     {
//       id: 3,
//       title: 'Içamento',
//       description: 'Temos uma equipe preparda para realizar serviços de içamento com segurança.'
//     },
//     {
//       id: 4,
//       title: 'Guarda móveis',
//       description: 'osso guarda-móveis é próprio para mudanças e tem segurança garantida, independente das necessidades do cliente.'
//     },
//   ])
// })

</script>

<template>
  <div class="container">
    <h2>Boas-vindas!</h2>
    <strong>Conheça os nossos serviços!</strong> <br />

    <!-- <template v-if="services.length > 0">

      <h3 v-for="service in services">{{ service.title }}</h3>
    </template> -->

    <RouterLink to="/">Sair</RouterLink>
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

h2 {
  margin-bottom: 0.6rem;
}

a {
  width: fit-content;
  padding: 0.4rem 0.8rem;
  border: 1px solid hsla(160, 100%, 37%, 1);
  border-radius: 8px;
}
</style>
