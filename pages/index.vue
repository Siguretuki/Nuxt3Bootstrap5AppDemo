<template>
    <div id="web">
        <Header />
        <Title/>
        <About />
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
import Title from "@/components/title.vue";
import About from "@/components/about.vue";
import Skill from "@/components/skill.vue";
import Footer from "@/components/footer.vue";
export default{
    components:{
        Header,
        Title,
        About,
        Skill,
        Footer,
    }
}
</script>