<template>
  <v-container>
    <v-toolbar color="transparent">
      <v-toolbar-title>
        <h3>Skills :</h3>
      </v-toolbar-title>
    </v-toolbar>
    <v-row>
      <v-col>
        <v-sheet
          v-for="skill in skillRange(0, 5)"
          :key="skill.id"
          color="transparent"
        >
          <v-sheet class="my-4">
            <h3 class="title">{{ skill.skill }}</h3>
            <ul class="tools-list">
              <li class="pa-2">
                {{ findSkill(skill.id).tools.join(", ") }}
              </li>
            </ul>
          </v-sheet>
        </v-sheet>
      </v-col>
      <v-col v-if="skills.length > 6">
        <v-sheet
          v-for="skill in skillRange(5, skills.length)"
          :key="skill.id"
          color="transparent"
        >
          <v-sheet class="my-4">
            <h3 class="title">{{ skill.skill }}</h3>
            <ul class="tools-list">
              <li class="pa-2">
                {{ findSkill(skill.id).tools.join(", ") }}
              </li>
            </ul>
          </v-sheet>
        </v-sheet>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import { computed } from "vue";
import { defineComponent } from "vue";

export default defineComponent({
  name: "skills-view",

  setup() {
    const skills = [
      {
        skill: "Web Essentials",
        tools: ["html", "css", "javascript"],
        id: "s-1",
      },
      {
        skill: "JavaScript Frameworks",
        tools: ["Vue.js", "React.js"],
        id: "s-2",
      },
      {
        skill: "State Managment",
        tools: ["Vuex", "React-Redux", "Pinia"],
        id: "s-3",
      },
      {
        skill: "Css Libraries",
        tools: ["TailwindCss", "BootStrap"],
        id: "s-4",
      },
      {
        skill: "Component Libraries",
        tools: ["Vuetify", "BootStrap-Vue"],
        id: "s-5",
      },
      {
        skill: "Design Principles",
        tools: ["Atomic Design", "StoryBook"],
        id: "s-6",
      },
      {
        skill: "Version Control Systems",
        tools: ["Git", "Git-Hub"],
        id: "s-7",
      },
      {
        skill: "Unit Test",
        tools: ["Vitest", "Jest"],
        id: "s-8",
      },
      {
        skill: "Build Tools",
        tools: ["WebPack", "Vite", "Babel"],
        id: "s-9",
      },
    ];

    const tools = computed(() => {
      return skills.map((skill) => skill.tools);
    });

    const findSkill = computed(() => {
      return function (id) {
        return skills.find((skill) => skill.id === id);
      };
    });

    const skillRange = computed(() => {
      return function (ini = 0, val) {
        return skills.slice(ini, val);
      };
    });

    return {
      skills,
      tools,
      findSkill,
      skillRange,
    };
  },
});
</script>

<style scoped>
.title {
  padding: 10px;
  border-bottom: 2px rgb(63, 63, 63) dashed;
  display: inline-block;
}

.tools-list {
  display: flex;
}
.tools-list > li {
  list-style: none;
}
</style>
