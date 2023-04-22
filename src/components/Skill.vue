<script setup lang="ts">
import type Skill from '../object/Skill';
defineProps<{
  data: Skill
}>()
function SkillLevel(level:number){
  let returnData =""
  switch (true) {
    case (level == 0):
      returnData= "Novice";
      break;
    case (level <=3):
      returnData = "Débutant avancé";
      break;
    case (level <=6):
      returnData = "Compétent";
      break;
    case (level < 10):
      returnData = "Professionnel";
      break;
    case (level <= 10):
      returnData = "Expert";
      break;
    default:
      returnData = "";
  }
  return returnData;
}
</script>

<template>
  <div class="greetings">
    <p class="green">{{ data.name }} - {{ data.type }} - {{ SkillLevel(data.level) }}</p>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {

  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
