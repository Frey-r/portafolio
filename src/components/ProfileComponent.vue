<script setup>
import GitIcon from "@/components/icons/IconGit.vue";
import PythonIcon from "@/components/icons/IconPython.vue";
import VueIcon from "@/components/icons/IconVue.vue";
import SpringIcon from "@/components/icons/IconSpring.vue";
import TechCard from "@/components/TechCard.vue";
import SQLIcon from "@/components/icons/IconSQL.vue";
import JavaIcon from "@/components/icons/IconJava.vue";
import JavascriptIcon from "@/components/icons/IconJavascript.vue";
import HtmlIcon from "@/components/icons/IconHtml.vue";
import CssIcon from "@/components/icons/IconCss.vue";
import AwsIcon from "@/components/icons/IconAws.vue";
import FlaskIcon from "@/components/icons/IconFlask.vue";
import PetryIcon from "@/components/icons/IconPoetry.vue";
</script>

<template>
  <div class="profile-component">
    <section class="profile-image-text">
      <div class="img-container">
        <img alt="Eduardo Bachmann Backend dev developer" class="profile-image" src="../assets/portfolio-portrait.webp">
      </div>
      <div class="profile-text">
        <h1 class = "profile-subtitle text-primary">
          Eduardo Bachmann
        </h1>
        <h1 class = "profile-subtitle text-secundary">
          Backend Developer
        </h1>
        <p class = "profile-paragraph text-base">
          2+ Años de experiencia
        </p>
        <div class="profile-tech">
          <TechCard class = "tech-card">
            <template #icon>
              <GitIcon />
            </template>
            <template #content>
              <span>Git</span>
            </template>
          </TechCard>
          <TechCard class = "tech-card">
            <template #icon>
              <PythonIcon />
            </template>
            <template #content>
              <span>Python</span>
            </template>
          </TechCard>
          <TechCard class = "tech-card">
            <template #icon>
              <VueIcon />
            </template>
            <template #content>
              <span>Vue</span>
            </template>
          </TechCard>
          <TechCard class = "tech-card">
            <template #icon>
              <SpringIcon />
            </template>
            <template #content>
              <span>Spring</span>
            </template>
          </TechCard>
          <TechCard class = "tech-card">
            <template #icon>
              <JavaIcon />
            </template>
            <template #content>
              <span>Java</span>
            </template>
          </TechCard>
          <TechCard class = "tech-card">
            <template #icon>
              <JavascriptIcon />
            </template>
            <template #content>
              <span>JS</span>
            </template>
          </TechCard>
          <TechCard class = "tech-card">
            <template #icon>
              <SQLIcon />
            </template>
            <template #content>
              <span>SQL</span>
            </template>
          </TechCard>
          <TechCard class = "tech-card">
            <template #icon>
              <HtmlIcon />
            </template>
            <template #content>
              <span>HTML</span>
            </template>
          </TechCard>
          <TechCard class = "tech-card">
            <template #icon>
              <CssIcon />
            </template>
            <template #content>
              <span>CSS</span>
            </template>
          </TechCard>
          <TechCard class = "tech-card">
            <template #icon>
              <AwsIcon />
            </template>
            <template #content>
              <span>AWS</span>
            </template>
          </TechCard>
          <TechCard class = "tech-card">
            <template #icon>
              <FlaskIcon />
            </template>
            <template #content>
              <span>Flask</span>
            </template>
          </TechCard>
          <TechCard class = "tech-card">
            <template #icon>
              <PetryIcon />
            </template>
            <template #content>
              <span>Poetry</span>
            </template>
          </TechCard>
        </div>
      </div>

    </section>
  </div>
</template>

<style scoped>
  .profile-image-text {
    display: flex;
    max-height: 80%;
    align-items: center;
    gap: 1rem;
    & .img-container{
      padding: 1rem .6em 0 0.6rem;
      background-color: var(--bt-c-text-secundary);
      display: flex;
      border-radius: .2rem;
      & img{
        max-height: 57svh;
        max-width: 100%;
      }
    }
    & .profile-text{
      display: flex;
      flex-direction: column;
      gap: 0.3rem;
      justify-content: center;
      & .profile-subtitle{
        font-weight: bold;
        line-height: 1;
      }
      & .text-primary{
        font-size: 2.5rem;
        color:var(--bt-c-text-primary);
      }
      & .text-secundary{
        color:var(--bt-c-text-secundary);
      }
      & .profile-tech{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        gap: 0.6rem;
        max-width: 100%;
        margin-top: 1rem;

        & .tech-card{

        }
      }
    }
  }
</style>