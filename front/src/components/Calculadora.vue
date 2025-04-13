<template>
    <div class="min-w-sm p-4 bg-white rounded-lg shadow-md">
        <div class="bg-gray-100 p-4 mb-4 text-center rounded-md text-gray-600 border-2 border-gray-300">
            {{ message }}
        </div>

        <div class="grid grid-cols-3 gap-2">
            <button v-for="number in 9" :key="number" @click="handleClick(number)"
                class="bg-gray-500 hover:bg-gray-600 text-white py-3 rounded-md text-lg border-4 border-gray-700/30">
                {{ number }}
            </button>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            message: 'Pulsa un número'
        }
    },
    methods: {
        handleClick(number) {
            this.message = `Has pulsado el número ${number}`;
        }
    }
}
</script>