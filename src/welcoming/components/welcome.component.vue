<script>
export default {
  name: "welcome",
  props: {
    firstName: String,
    lastName: String
  },

  methods: {
    developerName() {
      return this.firstName == null || this.lastName == null ? "Unknown" : `${this.firstName} ${this.lastName}`.trim();
    }
  }
}
</script>

<template>
  <p>Hello {{ developerName() }}. Now You are a Vue Developer!.</p>
</template>

