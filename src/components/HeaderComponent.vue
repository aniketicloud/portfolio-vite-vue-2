<template>
  <header>
    <div class="logo">
      <img
        alt="Vue logo"
        class="logo"
        src="@/assets/code.svg"
        width="48"
        height="48"
      />
      <h1>Nikefy</h1>
    </div>

    <nav>
      <router-link class="nav-link" data-item="Home" to="/">Home</router-link>
      <router-link class="nav-link" data-item="Projects" to="/projects"
        >Projects</router-link
      >
      <router-link class="nav-link" data-item="About" to="/about"
        >About</router-link
      >
    </nav>
  </header>
</template>

<style lang="scss" scoped>
.logo {
  display: grid;
  grid: auto-flow/1fr 1fr;
  align-items: center;
  gap: 0.5em;
  margin-top: 0.125em;

  img {
    justify-self: end;
  }

  h1 {
    font-family: "Bookerly Bold";
  }
}

nav {
  display: flex;
  justify-content: space-around;
  margin-top: 0.75em;

  .nav-link {
    text-decoration: none;
    color: #8f8f8f;
    font-family: "Bookerly";
    font-size: 24px;
    transition: all 0.5s ease-in-out;
    position: relative;
    text-transform: uppercase;

    &::before {
      content: attr(data-item);
      transition: 0.5s;
      color: #8254ff;
      position: absolute;
      top: 0;
      bottom: 0;
      left: 0;
      right: 0;
      width: 0;
      overflow: hidden;
    }

    &:hover {
      &::before {
        width: 100%;
        transition: all 0.5s ease-in-out;
      }
    }
  }

  .nav-link.router-link-exact-active.router-link-active {
    color: #8254ff;
  }
}
</style>
