<template>
    <div class="text-center bg-light" id="footer">
        <footer>{{data.footer}}</footer>
        <div id="link" v-for="item in data.sns_link">
            <a :href="item.text">
                <div>{{ item.name }}</div>
            </a>
        </div>
    </div>
</template>
<script setup>
    const data=useWeb()
</script>