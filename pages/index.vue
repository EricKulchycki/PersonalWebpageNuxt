<template>
  <div class="flex vert align">
    <Header title="who am i?">
      <div>
        <p>
          My name is Eric Kulchycki and I am a software developer that
          specializes in the web, with a focus on frontend development. I've
          worked with various web technologies, but React holds a special place
          in my heart.
        </p>
        <p>
          On this website you will find a showcase of my non-professional
          projects.
        </p>
      </div>
      <div class="flex socials">
        <a href="https://www.linkedin.com/in/ekulchycki/" target="_blank"
          ><font-awesome-icon :icon="faLinkedin" size="4x" class="icon"
        /></a>
        <a href="https://github.com/EricKulchycki" target="_blank"
          ><font-awesome-icon :icon="faGithub" size="4x" class="icon"
        /></a>
      </div>
    </Header>
  </div>
</template>

<script>
import { faLinkedin, faGithub } from "@fortawesome/free-brands-svg-icons";

export default {
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
.socials {
  margin-bottom: 2rem;
  margin-top: 2rem;
}

.icon {
  margin-right: 1rem;
  color: #90a4a4;
}
</style>
