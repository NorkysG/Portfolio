<script setup>
import { defineEmits } from "vue";

const emit = defineEmits(["toggle-aside"]);
</script>

<template>
  <nav class="navbar"> 
    <div class="divNav">
      <h1 class="h1Nav">Norkys</h1>

      <ul class="ul">
        <li class="lis"><a href="#home">Home</a></li>
        <li class="lis"><a href="#about">About</a></li>
        <li class="lis"><a href="#skills">Skills</a></li>
        <li class="lis"><a href="#projects">Projects</a></li>
        <li class="lis"><a href="#contact">Contact</a></li>
      </ul>

      <i class="fa-solid fa-bars menuIcon" @click="emit('toggle-aside')"></i>
    </div>
  </nav>
</template>

<style scoped>
.navbar {
  position: fixed;
  width: 100%;
  height: 65px;
  background: #000;
  display: flex;
  justify-content: center;
  z-index: 999;
}

.divNav {
  width: 100%;
  padding: 0 35px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.h1Nav {
  color: #a855f7;
  font-family: "Poppins", system-ui;
}

.ul {
  display: flex;
  gap: 45px;
  list-style: none;
}

.lis a {
  color: #fff;
  font-weight: 600;
  text-decoration: none;
  font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  font-size: 16px;
  transition: 0.2s;
}

.lis a:hover {
  color: #a855f7;
}

.menuIcon {
  display: none;
  color: white;
  font-size: 22px;
  cursor: pointer;
}


@media (max-width: 768px) {
  .ul {
    display: none;
  }

  .menuIcon {
    display: block;
    color: #f2f2f2;
  }
}
</style>
