<template>
    <div id="profile">
        <h2 class="container text-center p-2 pb-2 border-bottom">{{ data.about }}</h2>
        <div class="container">
            <div class="row align-items-center">
                <div class="col-3">
                    <img src="@/assets/img/myicon.jpg" alt="icon" class="my_icon rounded-circle my-5">
                </div>
                <div class="col-9">
                <dl class="row" v-for="item in data.profile">
                    <dt class="col-4 text-center">{{ item.text }}</dt>
                    <dd class="col-4">{{ item.contents }}</dd>
                </dl>
            </div>
            </div>
        </div>
        <div class="container">
            <div>
                <div class="p-3 d-flex align-items-center">
                    <p class="mb-0 lead">{{ data.comment }}</p>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
 const data = useWeb()
</script>