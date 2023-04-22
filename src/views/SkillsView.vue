<script setup lang="ts">
import skillList from '../data/skills.json';
import skillVue from '../components/Skill.vue'
</script>

name": "Node.js",
    "type": "Frameworks",
    "ico": "node.png",
    "level": 

<template>
        <div class="Skill">
          <h1>This is an Skill page</h1>
          <skillVue v-for="item in skillList" :data="item"></skillVue>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .Skill {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
