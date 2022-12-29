<template>
    <div id="web">
        <Header />
        <div class="container text-center">
            <h1>{{data.title}}</h1>
        <h3 class="text-center" v-for="item in data.subtitle">{{item.text}}</h3>
        </div>
        <About />
        <div class="container px-4">
            <div class="row gx-5">
                <div class="col">
                    <h2 class="p-3 border bg-light" v-for="item in data.blog">{{item.day}}</h2>
                </div>
                <div class="col">
                    <p class="p-3 border bg-light" v-for="item in data.blog">{{ item.contents }}</p>
                </div>
            </div>
        </div>
        <Skill/>
        <Footer/>
        <nuxt/>
    </div>
</template>
<script setup>
 const data = useWeb()
</script>
<script>
import Header from "@/components/header.vue";
import About from "@/components/about.vue";
import Skill from "@/components/skill.vue";
import Footer from "@/components/footer.vue";
export default{
    components:{
        Header,
        Footer,
        Skill,
    }
}
</script>