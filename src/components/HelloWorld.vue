<script setup lang="ts">
defineProps<{
  msg: string
}>()

// const width = 600
// const height = 400
// const imgUrl =
//   'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQAORfccCDlOsEHq-qQfY2una31CYsnzeO8cA&s'

const imageInfo = {
  width: 600,
  height: 400,
  imgUrl:
    'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQAORfccCDlOsEHq-qQfY2una31CYsnzeO8cA&s',
}
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      You’ve successfully created a project with
      <a href="https://vite.dev/" target="_blank" rel="noopener">Vite</a> +
      <a href="https://vuejs.org/" target="_blank" rel="noopener">Vue 3</a>. What's next?
    </h3>

    <!-- <img :src="imgUrl" alt="" :width="width" :height="height" /> -->
    <img v-bind="imageInfo" />
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
