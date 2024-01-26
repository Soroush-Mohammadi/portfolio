<template>
  <v-container>
    <v-row>
      <v-col>
        <v-toolbar color="transparent">
          <v-toolbar-title>
            <h3>Experiences :</h3>
          </v-toolbar-title>
        </v-toolbar>
        <v-divider thickness="2"></v-divider>
        <v-sheet color="transparent" class="mt-5">
          <h3 class="title">Freelance Front-End Developer | 3 Years</h3>
          <v-list class="my-5">
            <v-list-item>
              <li>
                Successfully completed numerous front-end development projects
                using Vue.js and React.js frameworks
              </li>
            </v-list-item>
            <v-list-item>
              <li>
                Collaborated with clients to gather requirements, provide
                technical guidance, and deliver customized solutions
              </li>
            </v-list-item>
            <v-list-item>
              <li>
                Developed responsive and visually appealing user interfaces,
                ensuring optimal user experience
              </li>
            </v-list-item>
            <v-list-item>
              <li>
                Implemented efficient and maintainable code, adhering to
                industry best practices and coding standards
              </li>
            </v-list-item>
          </v-list>
        </v-sheet>
      </v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-sheet color="transparent" class="mt-5">
          <h3 class="title">Intern | Moein Ertebate Pooya | 6 Months</h3>
          <v-list class="my-5">
            <v-list-item>
              <li>
                Contributed to the development of a web store application,
                working closely with senior developers to implement features and
                resolve issues
              </li>
            </v-list-item>
            <v-list-item>
              <li>
                Gained hands-on experience in front-end development, including
                HTML, CSS, JavaScript, and integration of third-party APIs
              </li>
            </v-list-item>
            <v-list-item>
              <li>
                Assisted with testing and debugging activities, ensuring
                application functionality and performance
              </li>
            </v-list-item>
          </v-list>
        </v-sheet>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "experineces-view",
};
</script>

<style scoped>
.title {
  display: inline-block;
  padding: 10px 0;
  border-bottom: 2px rgb(71, 71, 71) dashed;
}
</style>
