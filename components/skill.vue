<template>
    <div class="container" id="skill">
        <div class="row p-4">
            <h2 class="p-2 pb-2 border-bottom">{{ data.web_skill }}</h2>
            <div class="col p-3 text-center border border-info rounded-circle" v-for="item in data.skill">
                <h3>{{ item.text }}</h3>
                <p>{{ item.percentage }}</p>
            </div>
        </div>
        <div class="row p-4">
            <h2 class="p-2 pb-2 border-bottom">{{ data.programing_skill }}</h2>
            <div class="col p-3 text-center border border-info rounded-circle" v-for="item in data.programing">
                <h3>{{ item.text }}</h3>
                <p>{{ item.percentage }}</p>
            </div>
        </div>
        <div class="row p-4">
            <h2 class="p-2 pb-2 border-bottom">{{ data.dev_environment_skill }}</h2>
            <div class="col p-3 text-center border border-info rounded-circle" v-for="item in data.dev_environment">
                <h3>{{ item.text }}</h3>
                <p>{{ item.percentage }}</p>
            </div>
        </div>
        <div class="row p-4">
            <h2 class="p-2 pb-2 border-bottom">{{ data.other_skill }}</h2>
            <h3 class="col p-4 text-center border border-info rounded-circle" v-for="item in data.other">{{ item.text }}</h3>
        </div>
    </div>
</template>
<script setup>
 const data = useWeb()
</script>
