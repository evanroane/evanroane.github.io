<template>
  <nav class="nav">
    <NuxtLink class="nav-item" to="/">Home</NuxtLink>
    <span class="nav-spacer"></span>
    <NuxtLink class="nav-item" to="/about">About</NuxtLink>
    <span class="nav-spacer"></span>
    <a href="#" class="nav-item">Blog</a>
    <span class="nav-spacer"></span>
    <NuxtLink class="nav-item" to="/projects">Projects</NuxtLink>
    <span class="nav-spacer"></span>
    <NuxtLink class="nav-item" to="/contact">Contact</NuxtLink>
  </nav>
</template>

<style scoped>
.nav {
  margin: 1rem 0;
  padding: 1rem 0;
  border-top: 1px solid var(--white);
  border-bottom: 1px solid var(--white);
  display: flex;
  justify-content: center;
  align-content: center;
}

.nav-spacer:before {
  content: '\2043';
}

.nav-item {
  padding: 0 1em;
  color: var(--white);
  text-decoration: none;
}

.nav-item:link {
  color: var(--white);
}

.nav-item:visited {
  color: var(--white);
}

.nav-item:hover {
  color: var(--blue);
  text-decoration: underline;
}

.nav-item:active {
  color: var(--red);
}
</style>
