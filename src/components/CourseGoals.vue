<template>
  <ul>
    <li v-for="goal in goals" :key="goal">
      <slot :item="goal" text="..."></slot>
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      goals: ["Finish the cource!", "Learn Vue!", "Master the Vue!"],
    };
  },
};
</script>
