<template>
  <nav id="navbar" class="navbar">
    <img class="img-logo" src="@/assets/logo.svg" alt="" />

    <ul class="menu">
      <li><a href="#">Features</a></li>
      <li><a href="#mid">Team</a></li>
      <li><a href="#footer">Sign In</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "navbar",
};
</script>

<style scoped>
.navbar {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 0 2.5rem;
  font-size: clamp(0.8rem, 3vw, 1rem);
  font-family: var(--ft-secondary);
  width: 100%;
  max-width: 1500px;
}

.img-logo {
  justify-self: flex-start;
  width: clamp(5rem, 15vw, 9rem);
  margin: 1.5rem 0;
}
.menu {
  margin-left: auto;
  display: flex;
  justify-content: flex-end;
}
.menu li {
  margin: 0 1rem;
}
.menu li a {
  align-items: center;
  color: var(--dark-blue);
}
.menu li a:hover {
  opacity: 0.7;
}
@media screen and (max-width: 768px) {
  .navbar {
    padding: 0 1rem !important;
  }
}
</style>
