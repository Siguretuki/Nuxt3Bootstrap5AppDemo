<template>
    <div>
        <Header />
        <nuxt />
    </div>
    <div class="container">
        <h1 class="text-center">nuxt website</h1>
        <h3 class="text-center">田中 良日斗 6/21生まれ<br/>授業で制作したwebサイト<br/>Nuxt&Vue&BootStrapを使用</h3>
    </div>
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
    <div>
        <Footer/>
        <nuxt/>
    </div>
</template>
<script setup>
 const data = useWeb()
</script>
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