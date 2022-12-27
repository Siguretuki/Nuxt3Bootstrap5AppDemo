<template>
    <div>
        <Header/>
        <nuxt/>
    </div>
    <div>
        <h1>About Page</h1>
    </div>
    <div>
        <Footer/>
        <nuxt/>
    </div>
</template>
<script>
import Header from "@/components/header.vue";
import Footer from "@/components/footer.vue";
export default{
    components:{
        Header,
        Footer,
    }
}
</script>
