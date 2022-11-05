<template>
    <div>
        <header class="header">
            <slot name="header"></slot>
        </header>
        <main class="main">
            <slot name="main"></slot>
        </main>
        <footer class="footer">
            <slot name="footer"></slot>
        </footer>
    </div>
</template>

<script>
    export default{
        name: 'BaseLayout',
    }
</script>

<style>
    .header{
        color: white;
        background-color: black;
        padding: 40px;
        text-align: center;
    }
    .main{
        color: white;
        background-color: rgb(0, 17, 255);
        padding: 40px;
        text-align: center;
    }
    .footer{
        color: white;
        background-color: black;
        padding: 40px;
        text-align: center;
    }
</style>