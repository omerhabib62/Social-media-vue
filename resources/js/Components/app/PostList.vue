<script setup>
  import PostItem from "@/Components/app/PostItem.vue";
  const post1 = {
    user: {
      id: 1,
      name: "John Smith",
    },
    body: `
    <p>Adipisicing sint quis sit sunt sunt nisi. Proident elit reprehenderit eu id ut. Sit quis Lorem nostrud adipisicing tempor. Occaecat enim eiusmod aliqua in. Anim eiusmod aliquip incididunt laborum velit aliquip mollit nostrud nostrud laboris sint eiusmod qui.</p>

    <p>Adipisicing sint quis sit sunt sunt nisi. Proident elit reprehenderit eu id ut. Sit quis Lorem nostrud adipisicing tempor. Occaecat enim eiusmod aliqua in. Anim eiusmod aliquip incididunt laborum velit aliquip mollit nostrud nostrud laboris sint eiusmod qui.</p>
    `,
    created_by: "2023-11-19 15:12"
  }
</script>


<template>
  <div>    
    <PostItem :post="post1"/>
  </div>
</template>

<style scoped>

</style>

