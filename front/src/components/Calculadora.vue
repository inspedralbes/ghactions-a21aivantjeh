<template>
    <div class="calculator-box">
        <div class="display">
            {{ message }}
        </div>

        <div class="buttons">
            <button v-for="number in 9" :key="number" @click="handleClick(number)" class="btn">
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

<style>
.calculator-box {
    min-width: 300px;
    padding: 1rem;
    background-color: white;
    border-radius: 10px;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
}

.display {
    background-color: #f3f4f6;
    padding: 1rem;
    margin-bottom: 1rem;
    text-align: center;
    color: #4b5563;
    border: 2px solid #d1d5db;
    border-radius: 8px;
    font-size: 1rem;
}

.buttons {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 0.5rem;
}

.btn {
    background-color: #6b7280;
    color: white;
    padding: 0.75rem 0;
    border-radius: 8px;
    font-size: 1.125rem;
    border: 4px solid rgba(55, 65, 81, 0.3);
    cursor: pointer;
    transition: background-color 0.2s ease;
}

.btn:hover {
    background-color: #4b5563;
}
</style>