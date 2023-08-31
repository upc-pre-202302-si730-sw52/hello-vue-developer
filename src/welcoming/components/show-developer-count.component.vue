<script>
export default {
  name: "show-developer-count",
  data() {
    return {
      developerCount: 0
    };
  },
  methods: {
    onDeveloperRegistered(developer) {
      if (developer.fullName !== "Unknown")
        this.developerCount++;
    }
  }
}
</script>

<template>
  <div>
    <p>Developers registered: {{ developerCount }}</p>
    <p>Note: Unknown developers are not considered.</p>
  </div>
</template>
