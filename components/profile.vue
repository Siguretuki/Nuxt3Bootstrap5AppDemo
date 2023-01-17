<template>
    <div id="about">
        <h2 class="container text-center">{{ data.about }}</h2>
        <div class="container">
            <div class="row align-items-center">
                <div class="col-4">
                    <img src="@/assets/img/myicon.jpg" alt="icon" class="my_icon rounded-circle my-5">
                </div>
                <div class="col-8">
                <dl class="row" v-for="item in data.profile">
                    <dt class="col-4 text-center">{{ item.text }}</dt>
                    <dd class="col-4">{{ item.contents }}</dd>
                </dl>
            </div>
            </div>
        </div>
        <div class="container">
            <div>
                <div class="d-flex align-items-center">
                    <p class="mb-0 lead">{{ data.comment }}</p>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
 const data = useWeb()
</script>