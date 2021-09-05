<template>
  <div class="content">
    <div class="content__header">
      <img src="https://via.placeholder.com/50" alt="" />
      <p>GodMode</p>
    </div>

    <div class="content__sub">
      <p>Exclude</p>

      <div class="content__sub--card">
        <p>AXBDFE</p>
        <p>Png</p>
        <img src="https://via.placeholder.com/50" alt="" />
      </div>
    </div>

    <div class="content__events">
      <div class="content__events--card" v-for="i in 10" :key="i">
        <div class="content__events--card--left">
          <p>Coinbase</p>
          <p>40sec</p>
        </div>
        <div class="content__events--card--right">
          <a class="link" href="#">Token Transfer something something</a>
          <div class="token">
            <strong>Token:</strong>
            <p>DOGGY 550PG</p>
          </div>
          <div class="to-address">
            <strong>To Address:</strong>
            <p>0x223e238923829</p>
          </div>
          <div class="value">
            <strong>USD Value:</strong>
            <p>$1234</p>
          </div>
          <div class="from-address">
            <strong>From address:</strong>
            <p>0x223e238923829</p>
          </div>
        </div>
      </div>
    </div>
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

  &__header {
    display: flex;
    grid-gap: 1rem;
    padding: 1rem;

    p {
      margin: auto 0;
    }
  }

  &__sub {
    display: flex;
    flex-direction: column;
    grid-gap: 1rem;
    padding: 1rem;

    &--card {
      display: flex;
      grid-gap: 1rem;
      align-items: center;
      border: solid 1px black;
      padding: 1rem;
    }
  }

  &__events {
    display: flex;
    flex-direction: column;
    grid-gap: 1rem;
    border-top: 1px solid black;
    padding: 1rem;

    &--card {
      border: solid 1px black;
      display: grid;
      grid-template-columns: 100px 1fr;

      &--left {
        padding: 1rem;
        border-right: solid 1px black;
      }

      &--right {
        padding: 1rem;
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-gap: 1rem;
        grid-template-areas:
          "link link"
          "token to-address"
          "value from-address ";

        .link {
          grid-area: link;
          grid-gap: 1rem;
        }

        .token {
          grid-area: token;
          display: flex;
          grid-gap: 1rem;
        }

        .value {
          grid-area: value;
          display: flex;
          grid-gap: 1rem;
        }

        .to-address {
          grid-area: to-address;
          display: flex;
          grid-gap: 1rem;
        }

        .from-address {
          grid-area: from-address;
          display: flex;
          grid-gap: 1rem;
        }
      }
    }
  }
}
</style>
