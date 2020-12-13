<template>
  <div class="container">
    <div class="top flex justify align">
      <div class="flex vert align">
        <span class="text dev">&lt;/&gt;</span>
        <div class="name text">
          Eric Kulchycki
        </div>
        <div class="desc text">
          Software Developer
        </div>
      </div>
    </div>
    <div class="wave">
      <svg
        viewBox="0 0 500 150"
        preserveAspectRatio="none"
        style="height: 100%; width: 100%;"
      >
        <path
          d="M0.00,92.27 C216.83,192.92 304.30,8.39 500.00,109.03 L500.00,0.00 L0.00,0.00 Z"
          style="stroke: none; fill:#b4cdcd;"
        />
      </svg>
    </div>
  </div>
</template>

<style scoped>
.container {
  margin-bottom: 3rem;
}

.top {
  height: 300px;
  background-color: #b4cdcd;
}

svg {
  display: inline-block;
  position: absolute;
  top: 0;
  left: 0;
}
.wave {
  display: inline-block;
  position: relative;
  width: 100%;
  height: 150px;
  vertical-align: middle;
  overflow: hidden;
}

.text {
  color: white;
}

.name {
  font-size: 2.5rem;
  font-weight: 600;
}

.desc {
  font-size: 2rem;
}

.dev {
  font-size: 3rem;
  font-weight: bold;
  margin-bottom: 1rem;
}
</style>
