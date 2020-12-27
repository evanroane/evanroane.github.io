<template>
  <footer class="footer">&copy; Evan Roane {{currentYear}} All rights reserved</footer>
</template>

<script lang="ts">
export default {
  computed: {
    currentYear(): string {
      return String(new Date().getFullYear());
    }
  }
};
</script>

<style scoped>
.footer {
  margin-top: 2rem;
  font-size: 0.8rem;
  display: flex;
  justify-content: center;
}
</style>
