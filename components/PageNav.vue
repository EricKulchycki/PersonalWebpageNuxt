<template>
  <div style="margin-bottom: 2rem">
    <div class="grid page-nav">
      <NuxtLink to="/">
        home.
      </NuxtLink>
      <NuxtLink to="/about">
        about.
      </NuxtLink>
      <NuxtLink to="/projects">
        projects.
      </NuxtLink>
    </div>
    <el-divider />
  </div>
</template>

<style scoped>
.page-nav {
  grid-template-columns: repeat(3, 80px);
  column-gap: 1rem;
}

a {
  text-decoration: none;
  color: black;
  transition: 0.1s;
}
a:visited {
  color: inherit;
}
a:hover {
  color: #a6a6a6;
}
</style>
