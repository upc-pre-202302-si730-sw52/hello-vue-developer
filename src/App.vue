<script setup>
import Welcome from "./welcoming/components/welcome.component.vue";
import RegisterDeveloper from "./welcoming/components/register-developer.component.vue";
</script>

<template>
  <h1>Hello Vue Developer Application</h1>
  <register-developer />
  <welcome first-name="John" last-name="Doe" />
</template>

