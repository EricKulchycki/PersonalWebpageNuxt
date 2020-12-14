<template>
  <div>
    <div class="flex align">
      <p>
        <a
          href="http://bowlingsim.com"
          target="_blank"
        >bowlingsim</a> is a
        WebGL game built with JavaScript using the ThreeJS library and Physi.js
        library. It features physics, lighting, bump-mapping, and reflections.
      </p>
      <img
        id="bowling"
        src="bowling.png"
      >
    </div>
    <div class="flex tags">
      <TechTag
        v-for="(techName, index) in tech"
        :key="index"
        :name="techName"
      />
    </div>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      tech: ["javascript", "three-js", "physi-js"]
    };
  }
};
</script>

<style scoped>
#bowling {
  height: 100px;
  width: 100px;
  margin-left: 2rem;
  object-fit: cover;
  border-radius: 50%;
}

.tags {
  margin-top: 1rem;
  margin-bottom: 1rem;
}

a {
  text-decoration: none;
  font-weight: bold;
}
</style>
