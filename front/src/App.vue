<template>
  <div class="p-4 flex flex-col items-center justify-center min-h-screen bg-gray-100 gap-5">
    <p class="text-3xl font-bold border-b border-gray-400 text-gray-500">Calculadora</p>
    <Calculator />
    <p class="text-xs text-gray-400">Aivan Antonio</p>
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