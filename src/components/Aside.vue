<script setup>
import { ref } from "vue";

const props = defineProps({
  isOpen: Boolean,
});

const emit = defineEmits(["close"]);
</script>

<template>
  <div class="mobileAsideContainer">
    <aside class="mobileAside" :class="isOpen ? 'showAside' : 'hideAside'">
      <i class="fa-solid fa-arrow-left arrow-left" @click="emit('close')"></i>

      <ul class="ulContainer">
        <li class="lis">
          <a href="#home"><i class="fa-regular fa-house"></i> Home</a>
        </li>
        <li class="lis">
          <a href="#about"><i class="fa-regular fa-user"></i> About</a>
        </li>
        <li class="lis">
          <a href="#skills"><i class="fa-solid fa-code"></i> Skills</a>
        </li>
        <li class="lis">
          <a href="#projects"><i class="fa-solid fa-laptop"></i> Projects</a>
        </li>
        <li class="lis">
          <a href="#contact"><i class="fa-solid fa-at"></i> Contact</a>
        </li>
      </ul>
    </aside>
  </div>
</template>

<style lang="css" scoped>
.mobileAsideContainer {
  
  position: relative;
  z-index: 1000;
}

a {
  font-family:
    system-ui,
    -apple-system,
    BlinkMacSystemFont,
    "Segoe UI",
    Roboto,
    Oxygen,
    Ubuntu,
    Cantarell,
    "Open Sans",
    "Helvetica Neue",
    sans-serif;
  color: #f2f2f2;
  font-weight: 500;
  font-size: 18px;
  text-decoration: none;
  display: flex;
  align-items: center;
  gap: 10px;
  transition: 0.2s;
}

.arrow-left {
  position: absolute;
  top: 18px;
  right: 18px;
  font-size: 18px;
  color: #bbbbbb;
}

.mobileAside {
  width: 200px;
  height: 100vh;
  background-color: #080808;
  position: fixed;
  left: 0;
  padding-inline: 15px;
  padding-block: 50px;
}

.ulContainer {
  display: flex;
  flex-direction: column;
  text-decoration: none;
  list-style: none;
  gap: 40px;
}

.lis {
  padding-left: 10px;
  border-radius: 8px;
  padding-block: 6px;
  transition: 0.2s;
}

.lis:hover a {
  transform: translateX(10px);
}

.lis:hover {
  background-color: #181818;
}



@keyframes showAside {
  0% {
    transform: translateX(-300px);

  }

  100% {
    transform: translateX(0);
  }

}

.showAside {
  animation: showAside both ease-in-out 0.5s;
}

.hideAside {
  animation: hideAside both ease-in-out 0.5s;
}

 @keyframes hideAside {
  0% {
    transform: translateX(0);

  }

  100% {
    transform: translateX(-250px);
  }
}

@media (min-width: 768px) {
  .mobileAside {
    display: none;
  }
}
</style>
