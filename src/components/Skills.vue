<script setup></script>

<template>
  <section class="sectionSkills" id="skills">
    <div class="divSkillGeneral">
      <header class="headerSkills">
        <h1 class="h1Skill">Skills</h1>
        <p class="pSkill">Tools and technologies that bring creativity and life to every
          project.
            <i class="fa-solid fa-puzzle-piece iconSkillP"></i>
        </p>
      </header>
      <div class="articleGeneral">
        <div class="divSkillsArticle">
          <article class="articlesCard">
            <i class="fa-brands fa-html5 iconSkill"></i>
          </article>
          <article class="articlesCard">
            <i class="fa-brands fa-css3-alt iconSkill"></i>
          </article>
          <article class="articlesCard">
            <i class="fa-brands fa-js iconSkill"></i>
          </article>
        </div>

        <div class="divSkillsArticle">
          <article class="articlesCard">
            <i class="fa-brands fa-vuejs iconSkill"></i>
          </article>
          <article class="articlesCard">
            <i class="fa-brands fa-react iconSkill"></i>
          </article>
          <article class="articlesCard">
            <i class="fa-brands fa-git-alt iconSkill"></i>
          </article>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.sectionSkills {
  background-color: #050505;
  width: 100%;
  height: 500px;
}

.divSkillGeneral {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 50px;
}

.headerSkills {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px;
}

.h1Skill {
  color: #a855f7;
  font-family: "Poppins", system-ui;
}

.pSkill {
  color: #fff;
  font-family: "Poppins", system-ui;
}

.iconSkillP {
    font-size: 16px;
    color: #a855f7;
}

.articleGeneral {
  display: flex;
  flex-direction: column;
  gap: 35px;
}

.divSkillsArticle {
  display: flex;
  gap: 75px;
}
.iconSkill {
  color: #a855f7;
  font-size: 50px;
}

.articlesCard {
  width: 150px;
  height: 135px;
  background-color: #1a1a1a;
  border-radius: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
  box-shadow: 0 4px 15px rgba(155, 48, 255, 0.3);
  transition: 0.3s ease;
}

.articlesCard:hover {
  transform: scale(1.1);
}

@media (max-width: 768px) {
  .sectionSkills {
    justify-content: center;
    align-items: center;
    height: 100%;
  }
  .pSkill {
    width: 340px;
    text-align: center;
  }

  .divSkillsArticle {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
  }

  .articlesCard {
    width: 70px;
    height: 80px;
  }


}
</style>
