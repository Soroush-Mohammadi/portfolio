<template>
  <HelloWorld />
</template>

<script>
import { defineComponent } from "vue";
import HelloWorld from "@/components/HelloWorld.vue";
export default defineComponent({
  name: "Home-view",

  components: {
    HelloWorld,
  },
});
</script>
