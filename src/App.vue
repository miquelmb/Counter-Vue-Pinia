<template>
  <div class="app">
    <nav>
          <RouterLink to="/">Home</RouterLink> | 
          <RouterLink to="/about">About</RouterLink>
    </nav>
    <RouterView />
  </div>

</template>

<style>
nav {
  background-color: aquamarine;
  width: 400px;
  margin: auto;
  height: 50px;
  font-size: 16px;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.app {
  text-align: center;
}
</style>