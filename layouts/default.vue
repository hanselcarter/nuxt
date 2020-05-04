<template>
  <div>
    <TheHeader @sidenavToggle="display = !display" />
    <TheSideNav :show="display" @close="display = false" />
    <nuxt />
  </div>
</template>

<script>
import TheHeader from "@/components/navigation/TheHeader";
import TheSideNav from "@/components/navigation/TheSideNav";

export default {
  components: {
    TheHeader,
    TheSideNav
  },
  data() {
    return {
      display: false
    };
  }
};
</script>

<style>
html {
  font-family: "Open Sans", sans-serif;
}
body {
  margin: 0;
}
</style>
