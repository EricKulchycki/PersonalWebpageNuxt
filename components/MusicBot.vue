<template>
  <div>
    <div class="flex align">
      <img
        id="musicbot"
        src="note.png"
      >
      <p>
        <a
          href="https://github.com/EricKulchycki/MusicBot"
          target="_blank"
        >music bot</a> is an application made for use with slack. it is essentially just a flask api that accepts requests in
        the form of a link to an album, and returns links for that album on spotify, apple music, and google play music. the
        application was developed due to my coworkers sending links to music from their preferred streaming service, but everyone
        seemed to use different services. 
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
        "python",
      ]
    };
  }
};
</script>

<style scoped>
#musicbot {
  height: 100px;
  width: 100px;
  margin-right: 2rem;
  object-fit: cover;
}

.tags {
  margin-top: 1rem;
  margin-bottom: 1rem;
  flex-wrap: wrap;
}

a {
  text-decoration: none;
  font-weight: bold;
}
</style>