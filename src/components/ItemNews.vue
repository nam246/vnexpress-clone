<template>
  <div class="items-news">
    <h4>{{ title }}</h4>
    <div class="description">
        <img :src="img" alt="" v-if="img">
        <p>{{ description }}</p>
    </div>
  </div>
</template>

<script setup>
defineProps(['title', 'img', 'description'])
</script>

<style scoped>
.description {
    display: flex;
    margin: 12px 0;
}

.description p{
    padding-left: 12px;
    font-size: 14px;
}

.description img {
    width: 100%;
    height: 100%;
}
</style>