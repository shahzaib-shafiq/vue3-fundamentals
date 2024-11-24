<template>
  <div>
    <h1>Home</h1>
    <input type="text" placeholder="Email" v-model="email" />
    <br />
    <br />

    <input type="password" placeholder="Password" v-model="password" />
    <br />
    <br />

    <button @click="getData()">get Values</button>
  </div>
  {{ password }}
</template>

<script>
const getData = () => {
  return { email: null, password: null }
}
</script>
