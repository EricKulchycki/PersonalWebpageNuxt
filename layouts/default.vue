<template>
  <div>
    <Nav />
    <div class="flex justify">
      <div class="app-container">
        <PageNav />
        <Nuxt />
        <el-divider />
        <div class="flex socials">
          <a
            href="https://www.linkedin.com/in/ekulchycki/"
            target="_blank"
          ><font-awesome-icon
            :icon="faLinkedin"
            size="4x"
            class="icon"
          /></a>
          <a
            href="https://github.com/EricKulchycki"
            target="_blank"
          ><font-awesome-icon
            :icon="faGithub"
            size="4x"
            class="icon"
          /></a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { faLinkedin, faGithub } from "@fortawesome/free-brands-svg-icons";

export default {
  head() {
    return {
      title: "Eric Kulchycki"
    };
  },
  computed: {
    faLinkedin() {
      return faLinkedin;
    },
    faGithub() {
      return faGithub;
    }
  }
};
</script>

<style>
html {
  font-family: "Montserrat";
  line-height: 1.4rem;
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

.socials {
  margin-bottom: 2rem;
  margin-top: 2rem;
  justify-content: center;
}

.icon {
  margin-right: 1rem;
  color: #90a4a4;
}
</style>
