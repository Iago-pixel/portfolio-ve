<template>
  <TheHeader />
  <DefaultSection class="default-section"><p class="banner-text">BannerSection</p><TheButton class="banner-button">Button</TheButton></DefaultSection>
  <DefaultSection class="default-section"><p class="banner-text">AboutMeSection</p></DefaultSection>
  <SolidBorderSection>
    <template v-slot:title>TechSection</template>
    <DashedBox>
      <template v-slot:title>TechList</template>
      <ul class="tech-list">
        <TechCard>TechCard</TechCard>
        <TechCard>TechCard</TechCard>
        <TechCard>TechCard</TechCard>
        <TechCard>TechCard</TechCard>
      </ul>
    </DashedBox>
  </SolidBorderSection>
  <SolidBorderSection>
    <template v-slot:title>ProjectsSection</template>
    <DashedBox>
      <template v-slot:title>ProjectsList</template>
      <ul class="project-list">
        <ProjectCard>ProjectCard</ProjectCard>
        <ProjectCard>ProjectCard</ProjectCard>
        <ProjectCard>ProjectCard</ProjectCard>
        <ProjectCard>ProjectCard</ProjectCard>
      </ul>
    </DashedBox>
  </SolidBorderSection>
  <TheFooter />
</template>

<script>
import DashedBox from './components/DashedBox.vue';
import DefaultSection from './components/DefaultSection.vue';
import SolidBorderSection from './components/SolidBorderSection.vue';
import TheButton from './components/TheButton.vue';
import TheHeader from './components/TheHeader.vue'
import TechCard from './components/TechCard.vue';
import ProjectCard from './components/ProjectCard.vue';
import TheFooter from './components/TheFooter.vue';

export default {
  name: 'App',
  components: {
    TheHeader,
    TheButton,
    DefaultSection,
    SolidBorderSection,
    DashedBox,
    TechCard,
    ProjectCard,
    TheFooter
  }
}
</script>

<style>
#app {
  font-family: sans-serif;
  padding: 10px;
  max-width: 700px;
  margin: 0 auto;
}
body {
  background-color: black;
  margin: 0;
}
.default-section {
  display: flex;
  justify-content: center;
  align-content: center;
}
.banner-text {
  font-weight: bold;
}
.banner-button {
  position: absolute;
  left: 1rem;
  bottom: 1rem;
}
.tech-list {
  display: grid;
  grid-template-columns: auto auto auto;
  row-gap: 10px;
  column-gap: 20px;
  padding: 0;
}
.project-list {
  display: grid;
  grid-template-columns: auto auto;
  row-gap: 10px;
  column-gap: 20px;
  padding: 0;
}
</style>
