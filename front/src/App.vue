<template>
  <div class="container">
    <p class="title">Calculadora</p>
    <Calculator />
    <p class="author">Aivan Antonio</p>
  </div>
</template>

<script>
import Calculator from './components/Calculadora.vue'

export default {
  components: {
    Calculator
  }
}
</script>

<style>
.container {
  padding: 1rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  background-color: #f3f4f6;
  gap: 1.25rem;
}

.title {
  font-size: 1.875rem;
  /* 30px */
  font-weight: bold;
  border-bottom: 1px solid #9ca3af;
  color: #6b7280;
  margin-bottom: 0.5rem;
}

.author {
  font-size: 0.75rem;
  color: #9ca3af;
}
</style>