<script>
import Welcome from "./welcoming/components/welcome.component.vue";
import RegisterDeveloper from "./welcoming/components/register-developer.component.vue";
export default {
  name: "app",
  components: {Welcome, RegisterDeveloper},
  data() {
    return {
      firstName: '',
      lastName: ''
    }
    },
  methods: {
    onDeveloperRegistered(developer) {
      this.firstName = developer.firstName;
      this.lastName = developer.lastName;
      console.log("Developer registered: ", developer);
    }
  }

}

</script>

<template>
  <h1>Hello Vue Developer Application</h1>
  <register-developer v-on:developer-registered="onDeveloperRegistered" />
  <welcome :first-name="firstName" :last-name="lastName" />
</template>

