<template>
    <div class="text-center bg-light" id="footer">
        <footer class="p-2 pb-2">{{data.footer}}</footer>
        <div class="row justify-content-center">
            <div id="link" class="col-1" v-for="item in data.sns_link">
                <a class="btn btn-outline-primary btn-lg" :href="item.text" type="button">
                    {{ item.name }}
                </a>
            </div>
        </div>
    </div>
</template>
<script setup>
    const data=useWeb()
</script>