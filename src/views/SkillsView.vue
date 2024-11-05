<template>
  <div class="section">
    <h1>Technologies Studied</h1>
    <div class="container-one-backend">
      <!-- <h3 style="font-size: 2rem">Backend</h3> -->
      <div class="logos">
        <div class="icon-box icon-box-cyan">
          <a href="#">
            <div class="icon"></div>
            <h4 class="title">C#</h4>
            <img src="@/assets/Csharp.png" alt="" />
          </a>
          <p class="description">
            Explaining and writing new concepts and code snippets
          </p>
        </div>
        <div class="icon-box icon-box-cyan">
          <a href="#">
            <div class="icon"></div>
            <h4 class="title">Python</h4>
            <img src="@/assets/Python.png" alt="" />
          </a>
          <p class="description">
            Explaining and writing new concepts and code snippets
          </p>
        </div>
        <div class="icon-box icon-box-cyan">
          <a href="#">
            <div class="icon"></div>
            <h4 class="title">Vue.js</h4>
                        <img src="@/assets/vueing.png" alt="" />

          </a>
          <p class="description">
            Explaining and writing new concepts and code snippets
          </p>
        </div>
        <div class="icon-box icon-box-cyan">
          <a href="#">
            <div class="icon"></div>
            <h4 class="title">MSSQL</h4>
                        <img src="@/assets/database.jpg" alt="" />

          </a>
          <p class="description">
            Explaining and writing new concepts and code snippets
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.section {
  color: rgb(3, 3, 3);
}

.backend {
  display: flex;
  justify-content: center;
}

.logos img {
  box-shadow: 10px;
  height: 6rem;
}

.logos {
  display: flex;
  flex-wrap: wrap;
  justify-content:center;
  gap: 20px;
}

.icon-box a {
  color:blue;
  text-decoration: none;
}
.icon-box {
  border-radius:10px;
  padding: 30px;
  width: 23%;
  flex: 1 1 22%; /* Flexbox indstilling for bedre tilpasning */
  background-color: #fff;
  position: relative;
  overflow: hidden;
  margin: 0 0 40px 0;
  box-shadow: 0 5px 26px 0 rgba(68, 88, 144, 0.14);
  transition: all 0.3s ease-in-out;
  text-align: center;
  border: 1px solid #fff;
  min-width: 250px; /* Mindste bredde for at sikre god størrelse */
  max-width: 300px; /* Maksimal bredde for at bevare en konsekvent størrelse */

}

.icon-box::before {
  content: "";
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 4px;
  background-color: cyan;
  transform: scaleX(0);
  transition: transform 0.5s ease-in-out;
}
.icon-box:hover::before {
  transform: scaleX(1);
}
</style>