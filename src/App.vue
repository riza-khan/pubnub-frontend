<template>
  <div class="app">
    <div class="app__title">
      <h3>Godmode</h3>
    </div>
    <div class="app__body">
      <router-view />
    </div>
    <div class="app__footer">
      <p>Footer Content goes here</p>
    </div>
  </div>
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700&display=swap");

*,
*:before,
*:after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-size: 16px;
}

h1 {
  font-size: 3rem;
}

h3 {
  font-size: 2rem;
}

p {
  font-size: 1rem;
}

body {
  font-family: "Roboto", sans-serif;

  .app {
    display: flex;
    grid-gap: 1rem;
    flex-direction: column;
    justify-content: space-between;
    min-height: 100vh;

    &__title {
      border-bottom: solid 1px black;
    }

    &__body {
      margin-bottom: auto;
    }

    &__footer {
      border-top: solid 1px black;
    }
  }
}
</style>
