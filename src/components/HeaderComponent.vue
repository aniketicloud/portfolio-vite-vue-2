<template>
  <header>
    <div class="logo">
      <img
        alt="Vue logo"
        class="logo"
        src="@/assets/code.svg"
        width="125"
        height="125"
      />
      <h1>Nikefy</h1>
    </div>

    <div class="route-links">
      <nav>
        <router-link to="/">Home</router-link>
        <router-link to="/projects">Projects</router-link>
        <router-link to="/about">About</router-link>
      </nav>
    </div>
  </header>
</template>

<style lang="scss" scoped></style>
