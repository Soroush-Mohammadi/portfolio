<template>
  <v-navigation-drawer>
    <v-container
      fluid
      class="d-flex h-100 flex-column align-center justify-space-evenly"
    >
      <div class="header">
        <v-img
          src="/images/profile.png"
          width="150"
          class="rounded-circle bg-blue"
        ></v-img>
      </div>
      <div class="list text-center">
        <router-link v-for="route in routes" :key="route.id" :to="route.path">
          <v-list-item link :title="route.name"></v-list-item>
        </router-link>
      </div>
    </v-container>
  </v-navigation-drawer>
</template>

<style></style>

<script setup>
const routes = [
  {
    name: "Home",
    path: "/",
    id: "r1",
  },
  {
    name: "Experiences",
    path: "/experiences",
    id: "r2",
  },
  {
    name: "Projects",
    path: "/projects",
    id: "r3",
  },
  {
    name: "Skills",
    path: "/skills",
    id: "r4",
  },
];
</script>

<style scoped>
a {
  color: white;
  text-decoration: none;
}
</style>
