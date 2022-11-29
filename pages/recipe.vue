<template>
  <div class="container text-center my-5">
    <h1>{{ data.title }}</h1>
    <div class="alert alert-primary" role="alert">{{ data.description }}</div>
  </div>
  <div class="container mb-5">
    <div class="card mb-3 mx-auto">
      <div class="row g-0">
        <div class="col-md-4">
          <img
            src="https://img.cpcdn.com/recipes/3695776/894x1461s/03855e67f64548a05b1f995faabe8f57?u=12868943&p=1455726325"
            class="img-fluid rounded-start" alt="...">
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <h5 class="card-title">材料</h5>
            <div class="card-text">
              <ul>
                <li v-for="item in data.material">{{ item.text }}</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="container mb-5">
    <h2>作り方</h2>
    <div class="row row-cols-1 row-cols-sm-2 row-cols-md-4">
      <div class="col border p-2" v-for="item in data.recipe" :key="item.id">
        <div class="mb-2"><span class="badge bg-secondary">{{item.id}}</span></div>
        <p>{{item.text}}</p>
      </div>

    </div>
  </div>
  <div class="container mb-5">
    <div class="row gx-5">
      <div class="col-sm">
        <h3>コツ・ポイント</h3>
        <div v-for="item in data.point"><p>{{item.text}}</p></div>
      </div>
      <div class="col-sm">
        <h3>このレシピの生い立ち</h3>

        <p>今まで作ったKFCレシピは、卵液や粉もかなり余るし、何よりも
          何かひと味足りない……と思って、やっとKFC味にたどり着きました！</p>
        <p>どの家庭にもあるような材料で☆</p>
        <p>牛乳と卵液、粉類も必要量のみになっているので無駄が無く経済的です☆</p>
      </div>
    </div>
  </div>
</template>
<script setup>
 const data = useRecipe()
</script>
