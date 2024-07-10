<template>
    <div class="my-component">
        <h1 v-if="isVisible">{{ message }}</h1>
        <button v-on:click="isVisible = !isVisible">Cambiar visibilidad</button>
        <input v-model="message">
    </div>
</template>

<script>
export default {
    name: 'MyComponent',
    data(){
        return {
            message: 'Que onda gente',
            isVisible: true
        }
    },
    methods: {
        toggleVisibility(){
            this.isVisible = !this.isVisible;
        }
    }
}
</script>