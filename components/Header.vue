<template>
  <h2>{{ title }}</h2>
</template>

<script>
export default {
  name: "Header",
  props: {
    title: {
      type: String,
      default: ""
    }
  }
};
</script>
