<template>
  <v-img
    :src="src"
    :alt="alt"
    max-height="180px"
    max-width="180px"
    min-height="48px"
    min-width="48px"
  />
</template>

<script>
export default {
  name: "Knoten",
  props: {
    src: {
      type: String,
      required: true,
    },
    alt: {
      type: String,
      required: true,
    },
  },
};
</script>
