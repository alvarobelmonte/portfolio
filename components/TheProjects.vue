<template>
  <section class="projects-section">
    <h2 class="projects-title">Projects</h2>
    <main class="projects-list">
      <div class="project-card">
        <div class="project-img-container">
          <img class="project-img" src="~/static/projects/eduida-rec.png" alt="eduida" />
        </div>
        <div class="project-description-container">
          <h3 class="project-title">Eduida</h3>
          <p
            class="project-description"
          >Eduida es una plataforma para aprender inglés mientras juegas.</p>
          <h4 class="tech-title">Technologies</h4>
          <p class="project-tech">Nuxt, Strapi</p>
          <a class="project-button" href="https://eduida.es/">Demo</a>
        </div>
      </div>
    </main>
  </section>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.projects-section {
  min-height: 10rem;
}
.projects-title {
  background-color: transparent;
  text-align: center;
  font-weight: bold;
  font-size: 2rem;
  padding: 1rem;
}
.projects-list {
  display: flex;
  height: 100%;
  padding: 2rem 0;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background: rgb(203, 92, 107);
  background: linear-gradient(
    180deg,
    rgba(203, 92, 107, 0.5410539215686274) 0%,
    rgba(255, 174, 242, 1) 50%,
    rgba(255, 0, 65, 0.10127801120448177) 100%
  );
}
.project-card {
  width: 50%;
  display: flex;
  margin: 2rem 0;
  background-color: rgba(255, 255, 255, 0.55);
  border-radius: 1.5rem;
  -webkit-box-shadow: 0 2rem 5rem rgba(0, 0, 0, 0.1);
  -moz-box-shadow: 0 2rem 5rem rgba(0, 0, 0, 0.1);
  box-shadow: 0 2rem 5rem rgba(0, 0, 0, 0.1);
}
.project-img-container {
  background-color: transparent;
  width: 50%;
  padding: 2rem;
  display: flex;
  align-items: center;
  justify-content: center;
}
.project-description-container {
  padding: 2rem;
  width: 50%;
  background-color: transparent;
}
.project-title {
  color: black;
  text-align: center;
  font-weight: bold;
  padding: 0.5rem;
  font-size: 1.2rem;
  background-color: transparent;
}
.project-description {
  padding: 0.5rem 0;
  font-family: "Spartan", sans-serif;
  font-weight: 600;
  color: #2f2f2f;
  background-color: transparent;
  font-size: 0.9rem;
}
.project-img {
  width: 80%;
  border-radius: 2rem;
  transition: all 0.3s;
}
.project-img:hover {
  -moz-transform: scale(0.9) skew(-5deg, 3deg);
  -webkit-transform: scale(0.9) skew(-5deg, 3deg);
  -o-transform: scale(0.9) skew(-5deg, 3deg);
  -ms-transform: scale(0.9) skew(-5deg, 3deg);
  transform: scale(0.9) skew(-5deg, 3deg);
}
.tech-title {
  color: black;
  text-align: center;
  font-weight: bold;
  padding: 0.5rem;
  font-size: 1rem;
  background-color: transparent;
}
.project-tech {
  padding: 0.5rem 0;
  font-family: "Spartan", sans-serif;
  font-weight: 600;
  color: #2f2f2f;
  background-color: transparent;
}
.project-button {
  width: 100%;
  padding: 0.3rem;
  margin: 1rem 0;
  text-align: center;
  display: block;
  background-color: transparent;
  font-weight: bold;
  cursor: pointer;
  font-family: "Spartan", sans-serif;
  font-size: 0.9rem;
  text-decoration: none;
  &:hover,
  &:visited {
    color: tomato;
    text-decoration: none;
  }
}

@media only screen and (max-width: 720px) {
  .project-card {
    flex-direction: column;
    width: 90%;
    height: 100%;
  }
  .project-img-container {
    width: 100%;
    padding: 1rem;
  }
  .project-description-container {
    padding: 1.5rem;
    width: 100%;
  }
  .project-title {
    padding: 0.3rem;
    font-size: 1.1rem;
  }
}
@media only screen and (max-width: 1440px) {
  .project-img-container {
    width: 80%;
    padding: 1rem;
  }
}
</style>
