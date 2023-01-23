<template>
    <div class="container text-center bg-light" id="footer">
        <footer>{{data.footer}}</footer>
        <div id="link">
            <a v-bind="links">{{ data.name }}</a>
        </div>
    </div>
</template>
<script setup>
    const data=useWeb()
</script>