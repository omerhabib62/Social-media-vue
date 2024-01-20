<script setup>
  import PostItem from "@/Components/app/PostItem.vue";
  const post1 = {
    user: {
      id: 1,
      avatar: "https://randomuser.me/api/portraits/men/32.jpg",
      name: "John Smith",
    },
    group: null,
    attachments: [
      {
        id: 1,
        name: "test.png",
        url: "https://picsum.photos/1000",
        mime: "image/png",
      },
      {
        id: 2,
        name: "test2.png",
        url: "https://picsum.photos/1000",
        mime: "image/png",
      },
      {
        id: 3,
        name: "MyDocument.docx",
        url: "#",
        mime: "application/doc",
      }
    
    ],
    body: `
    <p>Adipisicing sint quis sit sunt sunt nisi. Proident elit reprehenderit eu id ut. Sit quis Lorem nostrud adipisicing tempor. Occaecat enim eiusmod aliqua in. Anim eiusmod aliquip incididunt laborum velit aliquip mollit nostrud nostrud laboris sint eiusmod qui.</p>

    <p>Adipisicing sint quis sit sunt sunt nisi. Proident elit reprehenderit eu id ut. Sit quis Lorem nostrud adipisicing tempor. Occaecat enim eiusmod aliqua in. Anim eiusmod aliquip incididunt laborum velit aliquip mollit nostrud nostrud laboris sint eiusmod qui.</p>
    `,
    created_at: "2023-11-19 15:12"
  }

  const post2 = {
    user: {
      id: 1,
      avatar: "https://randomuser.me/api/portraits/men/33.jpg",
      name: "Adam Smith",
    },
    group: {
      id: 1,
      name: "Laravel Developers"
    },
    body: `
    <p>Adipisicing sint quis sit sunt sunt nisi. Proident elit reprehenderit eu id ut. Sit quis Lorem nostrud adipisicing tempor. Occaecat enim eiusmod aliqua in. Anim eiusmod aliquip incididunt laborum velit aliquip mollit nostrud nostrud laboris sint eiusmod qui.</p>

    <p>Adipisicing sint quis sit sunt sunt nisi. Proident elit reprehenderit eu id ut. Sit quis Lorem nostrud adipisicing tempor. Occaecat enim eiusmod aliqua in. Anim eiusmod aliquip incididunt laborum velit aliquip mollit nostrud nostrud laboris sint eiusmod qui.</p>
    `,
    created_at: "2023-11-19 17:12"
  }
</script>


<template>
  <div class="overflow-auto">    
    <PostItem :post="post1"/>
    <PostItem :post="post2"/>
  </div>
</template>

<style scoped>

</style>

