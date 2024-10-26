<template>
  <v-container fluid class="h-75">
    <v-toolbar color="transparent">
      <v-toolbar-title>
        <h3>Introduction :</h3>
      </v-toolbar-title>
    </v-toolbar>
    <v-divider></v-divider>
    <v-container class="h-100 d-flex mt-10 flex-column justify-space-between">
      <v-sheet color="transparent">
        <v-row class="intro-body" align="center">
          <v-col class="profile-picture" cols="2">
            <v-img src="/images/my-profile.jpg" max-height="180"></v-img>
          </v-col>
          <v-col class="profile-details" cols="4">
            <h4>Name : Soroush mohamadi</h4>
            <h4>Email Address : mohamadysoroush@gmail.com</h4>
            <h4>
              Git Address :
              <a href="https://www.github.com/Soroush-Mohammadi">
                github.com/Soroush-Mohammadi
              </a>
            </h4>
            <h4>Occupation : Front-End Developer</h4>
          </v-col>
        </v-row>
      </v-sheet>
      <v-divider></v-divider>
      <v-sheet color="transparent">
        <h3>About Me :</h3>
        <p class="mt-6 text-body">
          Results-driven front-end developer with 5 years of experience
          specializing in utilizing popular frameworks such as Vue.js and
          React.js. Proficient in developing responsive and user-friendly web
          applications. Strong background as a freelancer, delivering
          high-quality projects for diverse clients. Previously worked as an
          intern, gaining hands-on experience in building a web store
          application. Currently seeking new opportunities as a front-end
          developer.
        </p>
      </v-sheet>
    </v-container>
  </v-container>
</template>

<script setup>
//
</script>

<style>
.text-body {
  line-height: 30px;
}
</style>
