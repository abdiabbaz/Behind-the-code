<template>
  <div class="about">
    <div class="header">
      <div class="main-container">
        <div class="container-one">
          <div class="profile">
            <img src="@/assets/Abdi.jpg" alt="" />
            <h3>Abdi Abbas</h3>
            <p>Computer Science Student</p>
          </div>
          <div class="social">
            <a href="https://github.com/abdiabbaz">
              <div class="link">
                <img src="@/assets/github.png" alt="" />
                <h2>Github</h2>
              </div>
            </a>
            <a href="https://www.linkedin.com/in/abdi-abbas-334a011a4/">
              <div class="link">
                <img src="@/assets/linkedin.png" alt="" />
                <h2>LinkedIn</h2>
              </div>
            </a>
          </div>
        </div>
        <div class="container-two">
          <div class="aboutme">
            <h1>About Me</h1>
            <p><i>Hello</i></p>
            <p>
              I am a dedicated Computer Science student at Zealand Roskilde with
              experience in multiple programming languages such as C#, Python,
              JavaScript, and Vue.js. My passion for technology and system
              development has led me to work on projects where I continuously
              explore new methods and technologies. I work with applications
              without database integration, focusing on creating user-friendly
              and efficient solutions.
            </p>
          </div>
          <div class="button-container">
            <div class="projects-button">
              <a href=""></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
export default {};
</script>

<style scoped>
img {
  height: 20px;
}

.main-container {
  display: flex;
  flex-direction: row;
  background-color: #ffffff;
  border-radius: 25px;
  padding-left: 20px;
  overflow: hidden;
  margin: 0 auto;
  width: 80%;
}

.container-one {
  background-color: #4a90e2;
  color: #2c3e50;
  padding: 2.5%;
  width: 30%;
  border-radius: 25px;
}

.profile img {
  height: 10rem;
  border-radius: 50%;
}

.container-two {
  /* background-color: #215fd3; */
  color: #2c3e50;
  width: 70%;
  margin: 2.5%;
  border-radius: 25px;
}

.social a {
  text-decoration: none;
  color: #2c3e50;
  font-size: 15px;
}

.social img {
  height: 3rem;
}

.aboutme {
  text-align: center;
}
</style>