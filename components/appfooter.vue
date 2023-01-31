<template>
    <div class="text-center bg-light" id="footer">
        <footer class="p-4 pb-2">{{data.footer}}</footer>
        <div class="row justify-content-center">
            <div id="link" class="col-1 p-4" v-for="item in data.sns_link">
                <div class="btn btn-outline-primary btn-lg" type="button" >
                    <a :href="item.text"  style="text-decoration:none;">
                    {{ item.name }}
                    </a>
                </div>
            </div>
        </div>
    </div>
</template>
<script setup>
    const data=useWeb()
</script>