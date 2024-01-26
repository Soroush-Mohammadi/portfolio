<template>
  <v-container>
    <v-toolbar color="transparent">
      <v-toolbar-title>
        <h3>Projects :</h3>
      </v-toolbar-title>
    </v-toolbar>
    <v-divider></v-divider>
    <v-row>
      <v-col>
        <v-sheet elevation="10" class="sheet pa-5">
          <h3 class="title">Online Store Project :</h3>
          <p>
            <span class="font-weight-black">Discription:</span><br />
            Developed and designed a feature-rich online store website
            encompassing a wide range of functionalities.
          </p>
          <p>
            <span class="font-weight-black"> Technologies Used: </span><br />
            Vue.js, Vue Router, Vuex, Vee-Validate, Vuetify, and Axios. Rest
            API's
          </p>
          <ul>
            <span class="font-weight-black">Key Features: </span
            ><br />
            <div class="pl-5">
              <li>
                User authorization system for secure access to the website.
              </li>
              <li>Form validation to ensure accurate and valid user input.</li>
              <li>Seamless AJAX integration for enhanced user experience.</li>
              <li>
                Payment system integration to facilitate secure online
                transactions.
              </li>
              <li>
                Search engine optimization techniques for improved visibility in
                search results.
              </li>
              <li>
                Mobile responsiveness ensuring optimal display on various
                devices.
              </li>
              <li>
                Ratings and reviews functionality for user feedback and
                engagement
              </li>
            </div>
          </ul>
        </v-sheet>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-sheet elevation="10" class="sheet pa-5">
          <h3 class="title">Pinterest Clone Project:</h3>
          <p>
            <span class="font-weight-black">Discription:</span><br />
            Developed a Pinterest clone website that emulates the core features
            and functionality of the popular social media platform. Users can
            register and log in to create and manage boards, save and organize
            images or links into pins, and follow other users and boards. The
            project aimed to provide a comparable user experience and interface
            while incorporating unique branding or customization.
          </p>
          <p>
            <span class="font-weight-black"> Technologies Used: </span><br />
            HTML, CSS, JavaScript, Vue.js, Pinia, Atomic Design, Vite, GraphQl,
            Story book
          </p>
          <ul>
            <span class="font-weight-black">Key Features: </span
            ><br />
            <div class="pl-5">
              <li>User registration and authentication system.</li>
              <li>Board creation, management, and organization.</li>
              <li>Pin creation, saving, and categorization.</li>
              <li>
                User profile management with the ability to follow other users.
              </li>
              <li>Responsive design for optimal viewing across devices.</li>
              <li>Integration of GraphQl for data retrieval and storage.</li>
              <li>
                Implementation of real-time updates for board and pin
                interactions.
              </li>
            </div>
          </ul>
        </v-sheet>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "projects-view",
});
</script>

<style scoped>
.title {
  display: inline-block;
  padding: 10px 0;
}

.sheet {
  line-height: 30px;
}
</style>
