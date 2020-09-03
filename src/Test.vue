<template>
  <div>
    {{ foo }}
    {{ name }}
  </div>
</template>

<script>
export default {
  name: "Test",
  props: ["foo", "bar"],
  data() {
    return {
      name: "Joe",
    };
  },
  computed: {
    upperName() {
      return this.name.toUpperCase();
    },
  },
};
</script>
