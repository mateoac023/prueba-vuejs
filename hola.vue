<template>
    <div>
        <p>Hola para la prueba</p>
        <div>{{ text }}</div>
    </div>
</template>

<script>
    export default {
        data(){
            return {
                text: "Hello world",
            };
        },
    };
</script>

<style>
p {
    color: red;
}
</style>