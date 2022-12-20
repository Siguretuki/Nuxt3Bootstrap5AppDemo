<template>
    <div id="web">
        <div class='container text-center'>
            <h1>{{data.title}}</h1>
        </div>
        <div class="container">
            <div class="row row-cols-1 row-cols-sm-2 row-cols-md-4">
                    <h2 v-for="item in data.blog">{{item.day}}</h2>
                    <div class="col border p-2">
                        <p v-for="item in data.blog">{{ item.contents }}</p>
                    </div>
            </div>
        </div>
    </div>
</template>
<script setup>
 const data = useWeb()
</script>