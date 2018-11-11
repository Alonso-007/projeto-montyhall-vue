<template>
    <div id="app">
        <h1>Problema de Monty Hall</h1>
        <!-- : serve para passar parametro false sem o : ia passar a string false -->
        <Door number="1" :hasGift="false" />
    </div>
</template>

<script>

    import Door from "./components/Door";

    export default {
        name: "App", //nao e obrigado mas ajuda na hora depurar o fonte
        components: { Door }
    }
</script>

<style>
    * {
        box-sizing: border-box;
        font-family: "Montserrat", sans-serif;
    }

    body {
        color: #FFF;
        background: linear-gradient(to right, rgb(21, 153, 87), rgb(21, 87, 153));
    }

    #app {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    #app h1 {
        border: 1px solid #000;
        background-color: #0004;
        padding: 20px;
        margin-bottom: 60px;
    }
</style>
