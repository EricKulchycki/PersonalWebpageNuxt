<template>
  <div>
    <Nav />
    <div class="flex justify">
      <div class="app-container">
        <PageNav />
        <Nuxt />
        <div />
      </div>
    </div>
  </div>
</template>

<style>
html {
  font-family: "Montserrat";
}

body {
  margin: unset;
}

.flex {
  display: flex;
}

.vert {
  flex-direction: column;
}

.justify {
  justify-content: center;
}

.space-evenly {
  justify-content: space-evenly;
}

.align {
  align-items: center;
}

.grid {
  display: grid;
}

.app-container {
  width: 100%;
  max-width: 800px;
  margin-right: 1rem;
  margin-left: 1rem;
}
</style>
