<template>
    <div class="container text-center">
            <h1>{{data.title}}</h1>
        <h3 class="text-center" v-for="item in data.subtitle">{{item.text}}</h3>
    </div>
</template>
<script setup>
 const data = useWeb()
</script>