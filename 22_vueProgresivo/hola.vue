<template>
    <div>
        <p>Texto de prueba de Hola.vue</p>
        <div>{{ text }}</div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                text: "Texto de un componente"
            }
        }
    }
</script>

<style>
    div {
        color: red;
    }
</style>