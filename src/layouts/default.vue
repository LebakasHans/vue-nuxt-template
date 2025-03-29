<template>
  <div class="layout">
    <header>
      <nav>
        <NuxtLink to="/">
          Home
        </NuxtLink> |
        <NuxtLink to="/about">
          About
        </NuxtLink>
      </nav>
    </header>

    <main>
      <slot />
    </main>

    <footer>
      <p>&copy; {{ new Date().getFullYear() }} - My Nuxt Template</p>
    </footer>
  </div>
</template>

<style scoped>
.layout {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
}

header {
  padding-bottom: 20px;
  border-bottom: 1px solid #eee;
  margin-bottom: 20px;
}

footer {
  margin-top: 40px;
  padding-top: 20px;
  border-top: 1px solid #eee;
  text-align: center;
  font-size: 14px;
}
</style>
