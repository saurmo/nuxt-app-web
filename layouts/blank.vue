<template>
  <v-app>

    <nuxt />

  </v-app>
</template>

<script>
export default {
  beforeMount() {
    console.log("axios", this.$axios);
    console.log("moment", this.$moment);
    console.log("cookie", this.$cookie);
  },
  data() {
    return {
      clipped: false,
      drawer: true,
      fixed: false,
      items: [
        { icon: "apps", title: "Welcome", to: "/" },
        { icon: "bubble_chart", title: "Inspire", to: "/inspire" }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: "Vuetify.js"
    };
  }
};
</script>
