<template>
  <div style="height: 100%;">
    <div class="landing">
      <div class="center">
        <div class="list">
          <h2>eric kulchycki</h2>
          <h5>software developer</h5>
          <a href="#content" v-smooth-scroll="{ duration: 1000, offset: -50 }">
            <i class="el-icon-arrow-down scroll-icon" />
          </a>
        </div>
      </div>
    </div>
    <div class="container"> 
      <div class="content" id="content">Nice</div>
    </div>
  </div>
</template>

<script>
import Logo from "~/components/Logo.vue";

export default {
  components: {
    Logo
  }
};
</script>

<style>
.container {
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: #31333c;
}

.list {
  display: flex;
  flex-direction: column;
  text-align: center;
}

.scroll-icon {
  margin-top: 50px;
  color: white;
}

.scroll-icon:hover {
  cursor: pointer;
}

.center {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  color: #f1f0f0;
  display: flex;
  justify-content: center;
  font-weight: 300;
  font-size: 60px;
  padding-top: 4em;
}

.landing {
  background: url("../assets/stars.jpg");
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  height: 95vh;
  width: 100%;
}

.content {
  background-color: #f1f0f0;
  width: 100%;
  height: 100%;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  height: 5em;
  font-weight: 300;
  font-size: 60px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
