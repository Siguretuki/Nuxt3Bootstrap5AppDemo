<template>
    <div class="container text-center">
        <div class="row">
            <h2>{{ data.web_skill }}</h2>
            <h3 class="col" v-for="item in data.skill">{{ item.text }}</h3>
        </div>
        <div class="row">
            <h2>{{ data.other_skill }}</h2>
            <h3 class="col" v-for="item in data.other">{{ item.text }}</h3>
        </div>
    </div>
</template>
<script setup>
 const data = useWeb()
</script>