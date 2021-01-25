<template>
  <div>
      <ul>
          <li>{{book.title}}:{{book.author}}</li>
          
      </ul>
  </div>
</template>

<script>
export default {
    name:"BookItem",
    props: ['book'],
}
</script>

<style scoped>

</style>