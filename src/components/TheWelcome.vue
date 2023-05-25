<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>My Skills:</template>
    <ul>
      <li>Ruby on Rails</li>
      <li>Wordpress</li>
      <li>PHP</li>
      <li>Python</li>
      <li>JavaScript</li>
      <li>React</li>
      <li>Vue.js | In Progress :)</li>
    </ul>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>My Education</template>
    <ul>
      <li>Masters of Science - Media Studies - Indiana University Bloomington</li>
      <li>Bachelors of Arts - Major in Communications / Minors in English and Journalism - Northern Illinois University</li>
    </ul>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Location</template>
    <ul>
      <li>Greater Chicago Area</li>
    </ul>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Hobbies</template>
    <ul>
      <li>Running</li>
      <li>Weight Lifting</li>
      <li>Coffee</li>
      <li>Guitar</li>
    </ul>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Thank you for visiting</template>
  </WelcomeItem>
</template>
