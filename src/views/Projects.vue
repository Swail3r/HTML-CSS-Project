<script setup>
const projects = [
  {
    title: 'Personal Portfolio Website',
    description:
      'A personal portfolio website built using HTML and CSS to showcase my skills and projects.',
    technologies: ['HTML', 'CSS']
  },
  {
    title: 'Online Clothing Store',
    description:
      'An online clothing store designed to showcase clothing products with a modern and user-friendly shopping experience.',
    technologies: ['HTML', 'CSS', 'JavaScript']
  },
  {
    title: 'CampusSwap ZA E-Commerce Store',
    description:
      'A student-focused e-commerce platform where users can buy, sell, and rent products such as textbooks and laptops.',
    technologies: ['Vue.js', 'Node.js', 'Express.js', 'MySQL']
  },
  {
    title: 'Python Mini Toolkit',
    description:
      'A collection of small Python scripts for automating common tasks.',
    technologies: ['Python']
  }
]
</script>

<template>
  <section class="page-section">
    <h1>My Projects</h1>

    <div class="projects-container">
      <div
        v-for="project in projects"
        :key="project.title"
        class="project-card"
      >
        <h3>{{ project.title }}</h3>

        <p>{{ project.description }}</p>

        <div class="technologies">
          <span
            v-for="technology in project.technologies"
            :key="technology"
          >
            {{ technology }}
          </span>
        </div>
      </div>
    </div>
  </section>
</template>