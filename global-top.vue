<template>
  <div v-if="$slidev.nav.currentPage > 1" class="corner-brands">
    <img src="/codex.png" alt="Codex" />
    <img src="/ailoveu.png" alt="AI Love You" />
  </div>
</template>

<style scoped>
.corner-brands {
  position: absolute;
  right: 1.5rem;
  bottom: 1.2rem;
  display: flex;
  align-items: center;
  gap: 0.6rem;
  opacity: 0.7;
}
.corner-brands img { height: 1.6rem; width: auto; }
</style>
