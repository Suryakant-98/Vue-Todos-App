<script setup>
import { RouterLink } from 'vue-router';

</script>
<template>
  <header>
    <nav class="container">
        <div class="branding">
            <h1>Vue Todos App</h1>
        </div>
        <ul class="nav-routes">
            <RouterLink to="/" exact-active-class="active">Home</RouterLink>
            <RouterLink to="/about" exact-active-class="active">About</RouterLink>
        </ul>
    </nav>
  </header>
</template>



<style lang="scss" scoped>
header {
  background-color: #f1f1f1;
  nav {
    display: flex;
    align-items: center;
    padding: 25px 16px;

    .branding {
      display: flex;
      align-items: center;
      gap: 8px;
      img {
        max-width: 50px;
      }

      h1 {
        font-size: 24px;
      }
    }

    .nav-routes {
      display: flex;
      flex: 1;
      justify-content: flex-end;
      gap: 12px;
      list-style: none;

      a {
        text-decoration: none;
        color: inherit;
      }
      .active {
        /* Your active page styling here */
        font-weight: bold;
        color: #41b080;
      }
    }
  }
}

</style>