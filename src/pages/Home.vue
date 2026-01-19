<script setup lang="ts">
import { ref, onMounted } from "vue";
import Nav from "../components/Nav.vue";
import Particles from "../components/Particles.vue";
import About from "../components/About.vue";
import Skills from "../components/Skills.vue";
import Projects from "../components/Projects.vue";
import Contact from "../components/Contact.vue";
import Aside from "../components/Aside.vue";

const fullText = "Welcome To My Porfolio";
const displayedText = ref("");
const typingSpeed = 60;

function typeEffect(index = 0) {
  if (index < fullText.length) {
    displayedText.value += fullText[index];
    setTimeout(() => typeEffect(index + 1), typingSpeed);
  }
}

onMounted(() => {
  typeEffect();
});

const isAsideOpen = ref(false);

const toggleAside = () => {
  isAsideOpen.value = !isAsideOpen.value;
};
</script>

<template>
  <Nav @toggle-aside="toggleAside"/>
  <Aside :isOpen="isAsideOpen" @close="toggleAside"/>
  <main class="mainContainer" id="home"> 
    <div class="particles-container">
      <Particles
        :particle-count="200"
        :particle-spread="10"
        :speed="0.1"
        :particle-colors="['#d8b4fe']"
        :move-particles-on-hover="false"
        :particle-hover-factor="1"
        :alpha-particles="false"
        :particle-base-size="100"
        :size-randomness="1"
        :camera-distance="20"
        :disable-rotation="false"
        class="w-full h-full"
      />
    </div>
    <div class="container-general">
      <div class="divTexts">
        <header class="headerHome">
          <h1 class="title">
            {{ displayedText }}<span class="cursor">|</span>
          </h1>
          <h2 class="h2Home">Frontend Developer</h2>
        </header>
        <p class="pHome">
          Passionate about digital development and design, creating experiences
          that inspire and connect with people.
        </p>
        <div class="divIcons">
          <i class="fa fa-code icons"></i>
          <i class="fa fa-laptop-code icons"></i>
          <i class="fa fa-code-branch icons"></i>
        </div>
        <div class="divBtons">
          <button class="bton1">Dowland CV</button>
          <button class="bton2">Contact me</button>
        </div>
      </div>
      <div>
        <img class="robot" src="../assets/img/Robot.webp" />
      </div>
    </div>
    <About />
    <Skills />
    <Projects />
    <Contact />
  </main>
</template>

<style scoped>

.particles-container {
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  left: 0;
  overflow: hidden;
  z-index: -10;
  background-color: #050505;
}

.container-general {
  position: relative;
  height: 586px;
  z-index: 10;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 50px;
}

.headerHome {
  display: flex;
  flex-direction: column;
  gap: 3px;
}

.divTexts {
  display: flex;
  flex-direction: column;
  gap: 16px;
}

.cursor {
  color: #fff;
  animation: blink 1s step-end infinite;
}
.title {
  font-family: "Poppins", system-ui;
  display: inline-block;
  background: linear-gradient(
    120deg,
    #ffffff 0%,
    #d8b4fe 25%,
    #a855f7 50%,
    #d8b4fe 75%,
    #ffffff 100%
  );
  background-size: 200% auto;
  color: transparent;
  background-clip: text;
  -webkit-background-clip: text;
  animation: shine 3s linear infinite;
}

.h2Home {
  color: #fff;
  font-family: "Poppins", system-ui;
}

@keyframes shine {
  to {
    background-position: 200% center;
  }
}

@keyframes blink {
  50% {
    opacity: 0;
  }
}

.pHome {
  color: #fff;
  font-family: "Poppins", system-ui;
  width: 450px;
}

.divIcons {
  display: flex;
  gap: 10px;
}

.icons {
  font-size: 15px;
  color: #fff;
  -webkit-text-stroke: 1px #a855f7;
  text-shadow:
    0 0 5px #a855f7,
    0 0 10px #a855f7,
    0 0 15px #a855f7;
}

.robot {
  width: 230px;
  animation: flotar 3s ease-in-out infinite;
}
@keyframes flotar {
  0% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-20px);
  }
  100% {
    transform: translateY(0px);
  }
}

.divBtons {
  display: flex;
  gap: 30px;
  margin-top: 20px;
}

.bton1 {
  color: #fff;
  width: 120px;
  height: 35px;
  background-color: #a855f7;
  font-family: "Poppins", system-ui;
  border: solid 2px rgb(67, 11, 100);
  border-radius: 10px;
  font-weight: bold;
  font-size: 15px;
  text-align: center;
  cursor: pointer;
  transition: 0.2s;
}

.bton1:hover {
  background-color: #8e3bdc;
}

.bton2 {
  color: #fff;
  width: 120px;
  height: 35px;
  background-color: #000;
  border: solid 2px #a855f7;
  font-family: "Poppins", system-ui;
  border-radius: 10px;
  font-weight: bold;
  font-size: 15px;
  text-align: center;
  cursor: pointer;
}

@media (max-width: 768px) {
  .container-general {
    padding-top: 50px;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 700px;
  }

  .divTexts {
    justify-content: center;
    align-items: center;
  }

  .h2Home {
    text-align: center;
  }

  .pHome {
    width: 330px;
    text-align: center;
  }

  .robot {
    width: 170px;
  }

  .headerHome {
    gap: 10px;
  }
}
</style>
