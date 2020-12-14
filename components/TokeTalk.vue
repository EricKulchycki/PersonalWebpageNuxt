<template>
  <div>
    <div class="flex align">
      <img
        id="toketalk"
        src="badge.png"
      >
      <p>
        <a
          href="http://toketalk.ca"
          target="_blank"
        >toketalk.ca</a> is a social network for users to
        share their cannabis preferences. the site was developed with the intent
        to learn to implement and deploy a fully featured web application.
      </p>
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
      tech: [
        "javascript",
        "react",
        "node",
        "express",
        "docker",
        "mysql",
        "nginx"
      ]
    };
  }
};
</script>

<style scoped>
#toketalk {
  height: 100px;
  width: 100px;
  margin-right: 2rem;
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
