<template>
    <div>
        <h2 class="container text-center">{{ data.about }}</h2>
        <div class="container">
            <div>
                <dl class="row" v-for="item in data.profile">
                    <dt class="col-4  text-center">{{ item.text }}</dt>
                    <dd class="col-8">{{ item.contents }}</dd>
                </dl>
            </div>
        </div>
        <div class="container">
            <p>{{ data.comment }}</p>
        </div>
    </div>
</template>
<script setup>
 const data = useWeb()
</script>