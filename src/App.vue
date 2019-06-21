<template lang="pug">
v-app
  v-navigation-drawer(app)
  Toolbar
  v-content
    v-container(fluid)
      router-view
  v-footer(app)
</template>

<script>
import Toolbar from "@/components/Toolbar";
export default {
  components: { Toolbar }
};
</script>


<style lang="stylus">
@import '~vuetify/src/stylus/main';</style>

