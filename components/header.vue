<template>
    <div>
        <header>
            <div id="home">
                <nav-bar />
                <nuxt />
            </div>
        </header>
    </div>
</template>
<script>
import NavBar from "@/components/nav.vue";
export default{
    components:{
        NavBar,
    }
}
</script>