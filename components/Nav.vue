<template>
  <div class="nav background">
    <el-row :gutter="20">
      <el-col :span="6">
        <div class="name">Eric Kulchycki</div>
      </el-col>
      <el-col :span="18">
        <div class="nav-flex">
          <nuxt-link to="/" class="nav-button">
            <div>
              <i class="el-icon-s-home nav-icon" />Home
            </div>
          </nuxt-link>
          <nuxt-link to="/about" class="nav-button">
            <div>
              <i class="el-icon-user-solid nav-icon" />About
            </div>
          </nuxt-link>
          <nuxt-link to="/projects" class="nav-button">
            <div>
              <i class="el-icon-folder nav-icon" />Projects
            </div>
          </nuxt-link>
        </div>
      </el-col>
    </el-row>
  </div>
</template>


<script>
export default {
  data() {
    return {
      activeIndex: "1",
      activeIndex2: "2",
      activeIndex3: "3"
    };
  },
  methods: {
    handleSelect(key, keyPath) {
      console.log(key, keyPath);
    }
  }
};
</script>

<style scoped>
.nav {
  color: #f1f0f0;
  background-color: transparent;
  height: 60px;
  width: 100%;
  text-decoration: none;
  font-size: 1.6em;
}

.background {
  background: url("../assets/stars.jpg");
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  width: 100%;
}

.name {
  font-weight: 800;
  letter-spacing: 0.2em;
  padding: 10px 20px 0;
}

.nav-button {
  font-size: 0.7em;
  margin-right: 15px;
  margin-top: 7px;
  padding: 10px;
  color: #f1f0f0;
  text-decoration: none;
}

.nav-button:hover {
  background-color: #607a8383;
  border-radius: 3px;
}

.nav-icon {
  margin-right: 5px;
}

.nav-flex {
  display: flex;
  justify-content: flex-end;
}
</style>