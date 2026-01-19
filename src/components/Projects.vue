<script setup></script>

<template>
  <section class="sectionProjects" id="projects">
    <div class="divContainerProjects">
      <header class="headerProjects">
        <h1 class="h1Projects">Projects</h1>
        <p class="pProjects">
          Check out my projects and see how I bring ideas to life with code.
          <i class="fa-solid fa-folder folder"></i>
        </p>
      </header>
      <div class="divArticleProjects">
        <article class="articleProjects">
          <img class="imgBotana" src="../assets/img/FlowUpNorkys.webp" />
          <div class="info">
            <div class="info-skills">
              <div class="info2">
                <h2 class="h2Projects">FlowUp Social Network</h2>
                <p class="infoP">
                  FlowUp is a social network designed to connect people, share
                  ideas, and foster creativity in a modern and intuitive
                  environment.
                </p>
              </div>
              <div class="divSkills">
                <img class="imgProjects" src="../assets/svg/html.svg" />
                <img class="imgProjects" src="../assets/svg/css.svg" />
                <img class="imgProjects" src="../assets/svg/javascript.svg" />
                <img class="imgProjects" src="../assets/svg/Vue.svg" />
                <img class="imgProjects" src="../assets/svg/vite.svg" />
              </div>
            </div>
            <div class="btonsRepo">
              <a
                href="https://github.com/tu-usuario/tu-repositorio"
                target="_blank"
                rel="noopener noreferrer"
                class="btonProjects"
              >
                Repository
                <i class="fa-brands fa-github iconGitH"></i>
              </a>
            </div>
          </div>
        </article>

        <article class="articleProjects">
          <img class="imgBotana" src="../assets/img/BotanaWeb.webp" />
          <div class="info">
            <div class="info-skills">
              <div class="info2">
                <h2 class="h2Projects">Botana Website</h2>
                <p class="infoP">
                  A responsive website that offers complete information about
                  the business, including its services, points of sale and
                  values
                </p>
              </div>
              <div class="divSkills">
                <img class="imgProjects" src="../assets/svg/html.svg" />
                <img class="imgProjects" src="../assets/svg/css.svg" />
                <img class="imgProjects" src="../assets/svg/javascript.svg" />
                <img class="imgProjects" src="../assets/svg/Vue.svg" />
                <img class="imgProjects" src="../assets/svg/vite.svg" />
              </div>
            </div>
            <div class="btonsRepo">
              <a
                href="https://github.com/dualsoftSRL/Botana"
                target="_blank"
                rel="noopener noreferrer"
                class="btonProjects"
              >
                Repository
                <i class="fa-brands fa-github iconGitH"></i>
              </a>
            </div>
          </div>
        </article>

        <article class="articleProjects">
          <img class="imgBotana" src="../assets/img/Roseluxe.webp" />
          <div class="info">
            <div class="info-skills">
              <div class="info2">
                <h2 class="h2Projects">Roseluxe cosmetics website</h2>
                <p class="infoP">
                  A responsive website that offers complete information about
                  the business, including its services, points of sale and
                  values
                </p>
              </div>
              <div class="divSkills">
                <img class="imgProjects" src="../assets/svg/html.svg" />
                <img class="imgProjects" src="../assets/svg/css.svg" />
                <img class="imgProjects" src="../assets/svg/javascript.svg" />
                <img class="imgProjects" src="../assets/svg/Vue.svg" />
                <img class="imgProjects" src="../assets/svg/vite.svg" />
              </div>
            </div>
            <div class="btonsRepo">
              <a
                href="https://github.com/NorkysG/Roseluxe"
                target="_blank"
                rel="noopener noreferrer"
                class="btonProjects"
              >
                Repository
                <i class="fa-brands fa-github iconGitH"></i>
              </a>
            </div>
          </div>
        </article>
      </div>
    </div>
  </section>
</template>

<style scoped>
.sectionProjects {
  background-color: #050505;
  width: 100%;
  height: 580px;
}

.divContainerProjects {
  display: flex;
  flex-direction: column;
  gap: 65px;
}

.headerProjects {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 8px;
}

.h1Projects {
  color: #a855f7;
  font-family: "Ppoppins", system-ui;
}

.pProjects {
  color: #fff;
  font-family: "Poppins", system-ui;
}

.folder {
  color: #a855f7;
}

.divArticleProjects {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 30px;
}

.articleProjects {
  box-shadow: 0 4px 15px rgba(155, 48, 255, 0.3);
  width: 300px;
  height: 420px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  padding-top: 0;
  overflow: hidden;
  gap: 13px;
  border-radius: 10px;
}

.imgBotana {
  width: 100%;
  height: 150px;
  display: block;
}

.info {
  height: 100%;
  padding: 15px;
  padding-bottom: 30px;
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  gap: 25px;
}

.info-skills {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.info2 {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.h2Projects {
  font-family: "Poppins", system-ui;
  color: #fff;
  font-size: 18px;
}

.infoP {
  color: #c4c4c4;
  font-family: "Poppins", system-ui;
  font-size: 15px;
}

.divSkills {
  display: flex;
  gap: 18px;
  width: 100%;
  flex-wrap: wrap;
}

.imgProjects {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 27px;
  font-family: "Poppins", system-ui;
  border-radius: 5px;
}

.btonProjects {
  width: 128px;
  height: 35px;
  border-radius: 8px;
  background-color: #000;
  color: #fff;
  border: solid 1px #a855f7;
  box-shadow: 0 0 10px #a855f7;
  border-radius: 10px;
  cursor: pointer;
  font-family: "Poppins", system-ui;
  font-weight: bold;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 14px;
  gap: 5px;
  text-decoration: none;
}

.btonsRepo {
  align-self: flex-end;
  display: flex;
  justify-content: center;
  align-items: center;
}

.iconGitH {
  font-size: 20px;
}

.divArticleProjects:hover .articleProjects {
  filter: blur(2px);
  opacity: 0.6;
  transition: 0.3s ease;
}

.divArticleProjects:hover .articleProjects:hover {
  filter: blur(0);
  opacity: 1;
}

@media (max-width: 768px) {
  .sectionProjects {
    height: auto;
    padding-block: 35px;
  }

  .pProjects {
    text-align: center;
    width: 320px;
  }

  .divArticleProjects {
    flex-direction: column;
    gap: 38px;
  }
}
</style>
