<script setup>
const articles=[{title :"A article",
id:1}, {title:"B article",id:2},{title:"C article",id:3}]
</script>

<template>
  <div>
    <h1>Articles</h1>
    <NuxtLink :to="{name:'articles-id',params:{id: article.id, title: article.title}}" v-for="article of articles" :key="article.id">
        <div>
            {{ article.title }}
        </div>
    </NuxtLink>
  </div>
</template>

<style scoped>
</style>