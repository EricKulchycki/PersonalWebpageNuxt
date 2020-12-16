<template>
  <div
    class="tag"
    :class="classes"
  >
    {{ name }}
  </div>
</template>

<script>
export default {
  name: "TechTag",
  props: {
    name: {
      type: String,
      default: ""
    }
  },
  data: function() {

    const javascriptFrameworks = [
        "javascript",
        "express",
        "physi-js",
        "three-js"
      ];

    return {
      classes: {
        javascript: javascriptFrameworks.find(fr => fr === this.name),
        react: this.name === "react",
        node: this.name === "node",
        docker: this.name === 'docker',
        mysql: this.name === 'mysql',
        nginx: this.name === 'nginx',
        python: this.name === 'python',
      }
    };
  }
};
</script>

<style>
.tag {
  border: 2px solid #e6e6e6;
  border-radius: 16px;
  padding: 0.5rem;
  margin-right: 0.5rem;
  margin-top: 0.5rem;
  background-color: #f8f8f8;
  font-weight: bold;
  color: #333;
}

.javascript {
  border-color: #b0b000;
  color: #b0b000;
  background-color: #ffffec;
}

.react {
  border-color: #00c7eb;
  color: #007489;
  background-color: #d8f9ff;
}

.node, .nginx {
  border-color: #3c9e5b;
  background-color: #b3e0a2;
  color: #333;
}

.docker {
  border-color: #506d77;
  background-color: #8bdef9;
  color: #384d54;
}

.mysql {
  border-color: #d88c00;
  background-color: #caf6ff;
  color: #d88c00;
}

.python {
  border-color: #306998;
  background-color: #cddfed;
  color: #333;
}
</style>
