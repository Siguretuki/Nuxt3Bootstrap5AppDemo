<template>
    <div class="container text-center" id="skill">
        <div class="row">
            <h2>{{ data.web_skill }}</h2>
            <div class="col" v-for="item in data.skill">
                <h3>{{ item.text }}</h3>
                <p>{{ item.percentage }}</p>
            </div>
        </div>
        <div class="row">
            <h2>{{ data.programing_skill }}</h2>
            <div class="col" v-for="item in data.programing">
                <h3>{{ item.text }}</h3>
                <p>{{ item.percentage }}</p>
            </div>
        </div>
        <div class="row">
            <h2>{{ data.dev_environment_skill }}</h2>
            <div class="col" v-for="item in data.dev_environment">
                <h3>{{ item.text }}</h3>
                <p>{{ item.percentage }}</p>
            </div>
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
