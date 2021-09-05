<template>
  <div class="content">
    <div class="content__header">
      <img src="https://via.placeholder.com/50" alt="" />
      <p>GodMode</p>
    </div>

    <h1>Content goes here</h1>
    <p>
      Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ipsa, fugit
      nulla odit quae aliquid doloribus exercitationem quo reprehenderit
      laudantium ut voluptatibus quasi vitae nisi voluptates laborum sequi,
      impedit, rem adipisci? Lorem ipsum dolor sit, amet consectetur adipisicing
      elit. Nemo est labore rerum sunt consequuntur. Tenetur quibusdam est
      temporibus, iusto, optio ipsam similique nihil veniam minus libero
      distinctio ex facere vero. Lorem ipsum dolor sit amet consectetur
      adipisicing elit. Optio ratione quidem praesentium dolores quos? Aliquam
      adipisci numquam ea libero distinctio nisi odit voluptatibus esse tempora
      fugit. Eveniet magni mollitia culpa!
    </p>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "Home",
});
</script>

<style lang="scss" scoped>
.content {
  display: flex;
  grid-gap: 1rem;
  flex-direction: column;
  padding: 1rem;

  &__header {
    display: flex;
    grid-gap: 1rem;

    p {
      margin: auto 0;
    }
  }
}
</style>
