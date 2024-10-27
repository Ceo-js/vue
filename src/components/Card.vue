

<script lang="ts">
   export default {
      data() {
         return {
            user: {
               name: "",
               id: 0,
               email: "",
            }
         }
      },
      methods: {
      },
      props: {
         user: Object,
      },
   }
</script>

<template>
   <div class="kard">
      <div class="t" v-text="user.name"></div>
      <div>email: {{ user.email }}</div>
      <div>id: {{ user.id }}</div>
   </div>
</template>

<style scoped>
   .kard {
      display: flex;
      flex-direction: column;
      padding: 1em;
      border-radius: 24px;
      background: #e5e5e5;
   }

   .kard .t {
      color: #f0a;
      font-size: 2em;
      font-weight: bold;
   }
</style>