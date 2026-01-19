<script setup></script>

<template>
  <section class="sectionAbout" id="about">
    <div class="divAbout">
      <header class="headerAbout">
        <h1 class="h1About">About Me</h1>
        <p class="pAboutTitle">
          Transforming ideas into unique digital experiences.
          <i class="fa-regular fa-lightbulb icon"></i>
        </p>
      </header>
      <div class="divTextsAbout">
        <img class="perfil" src="../assets/img/foto.webp" />
        <span class="span">Software Engineer</span>
        <p class="aboutMe">
          I'm a Software Development student at ITLA (Instituto Tecnológico de
          Las Américas)<br />with one year of experience. I'm passionate about
          web development and enjoy <br />creating modern, functional, and
          visually appealing digital experiences.
        </p>
      </div>
      <div class="divArticles">
        <article class="articles">
          <i class="fa-solid fa-code iconAbout"></i>
          <h2 class="h2About">Creativity</h2>
          <p class="qualities">
            I bring innovative ideas to design and implementation, making each
            project unique.
          </p>
        </article>
        <article class="articles">
          <i class="fa-solid fa-brain iconAbout"></i>
          <h2 class="h2About">Problem Resolving</h2>
          <p class="qualities">
            I enjoy tackling challenges in coding and finding effective
            solutions efficiently.
          </p>
        </article>
        <article class="articles">
          <i class="fa-solid fa-magnifying-glass iconAbout"></i>
          <h2 class="h2About">Attention to Detail</h2>
          <p class="qualities">
            I focus on clean code, responsive layouts, and polished UI/UX for
            every project.
          </p>
        </article>
      </div>
    </div>
  </section>
</template>

<style scoped>
.sectionAbout {
  display: flex;
  flex-direction: column;
  background-color: #050505;
  width: 100%;
  height: 790px;
}

.divAbout {
  display: flex;
  flex-direction: column;
  justify-content: center;
  gap: 45px;
}

.headerAbout {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 5px;
}

.h1About {
  color: #a855f7;
  font-family: "Poppins", system-ui;
}

.texts {
  display: flex;
  align-items: center;
}

.pAboutTitle {
  color: #fff;
  font-size: 17px;
  font-family: "Poppins", system-ui;
}

.icon {
  color: #a855f7;
}

.divTextsAbout {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 18px;
  font-size: 20px;
}

.perfil {
  width: 200px;
  border-radius: 100%;
  border: solid 1px #a855f7;
  box-shadow: 0 0 25px #a855f7;
}

.span {
  width: 17ch;
  color: #a855f7;
  font-family: "Poppins", system-ui;
  text-wrap: nowrap;
  overflow: hidden;
  animation: typing 2s steps(20) infinite alternate-reverse;
  font-weight: bold;
}

@keyframes typing {
  from {
    width: 0ch;
  }
}

.aboutMe {
  color: #fff;
  font-family: "Poppins", system-ui;
  text-align: center;
  font-size: 18px;
}

.iconAbout {
  color: #a855f7;
  font-size: 27px;
}

.h2About {
  color: #fff;
  font-size: 17px;
  font-family: "Poppins", system-ui;
}

.qualities {
  color: #fff;
  font-size: 14x;
  font-family: "Poppins", system-ui;
  text-align: center;
}

.divArticles {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 40px;
}

.articles {
  width: 255px;
  height: 180px;
  border: solid 1px #a855f7;
  box-shadow: 0 0 10px #a855f7;
  border-radius: 10px;
  display: flex;
  padding-inline: 10px;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 8px;
}

@media (max-width: 768px) {
  .sectionAbout {
    width: 100%;
    height: auto;
  }

  .headerAbout {
    gap: 10px;
  }

  .aboutMe {
    width: 370px;
  }

  .pAboutTitle {
    width: 290px;
    text-align: center;
  }

  .divArticles {
    flex-direction: column;
  }
}
</style>
