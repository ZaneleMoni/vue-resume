<template>
  <hr />
  <div id="skill">
    <h1>Skills</h1>
    <div class="underline"></div>

    <div class="row">
      <div id="main" class="col-3">
        <div class="logo">
          <h6 class="skilling">JavaScript</h6>
          <p>
            <img
              src="https://media.vlpt.us/images/soom/post/6d36a847-bd07-479a-9953-76cdc9e5afe2/6288755792019456.jpeg"
              alt=""
              height="50px"
              class="text-center"
            />
          </p>
        </div>
      </div>
      <div id="main" class="col-3">
        <div class="logo">
          <h6 class="skilling">HTML</h6>
          <p>
            <img
              src="https://www.seekpng.com/png/detail/80-803527_html5-css3-and-javascript-logos-html5-logo-png.png"
              alt=""
              height="50px"
              class="text-center"
            />
          </p>
        </div>
      </div>
      <div id="main" class="col-3">
        <div class="logo">
          <h6 class="skilling">Bootstrap</h6>
          <p>
            <img
              src="https://i.stack.imgur.com/dMXbE.png"
              alt=""
              height="50px"
              class="text-center"
            />
          </p>
        </div>
      </div>
    </div>

    <div class="row">
      <div id="main" class="col">
        <div class="logo">
          <h6 class="skilling">CSS</h6>
          <p>
            <img
              src="https://e7.pngegg.com/pngimages/893/87/png-clipart-cascading-style-sheets-logo-css3-html-css3-logo-blue-angle.png"
              alt=""
              height="50px"
              class="text-center"
            />
          </p>
        </div>
      </div>
      <div id="main" class="col-3">
        <div class="logo">
          <h6 class="skilling">MySql</h6>
          <p>
            <img
              src="https://www.freepnglogos.com/uploads/logo-mysql-png/logo-mysql-mysql-logo-png-images-are-download-crazypng-21.png"
              alt=""
              height="50px"
              class="text-center"
            />
          </p>
        </div>
      </div>
      <div id="main" class="col-3">
        <div class="logo">
          <h6 class="skilling">Vue.js</h6>
          <p>
            <img src="https://vuejs.org/images/logo.png" alt="" height="50px" />
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
#main {
  padding: 10px 0 10px 0;
  margin: 10px;
  display: inline-block;
  justify-content: center;
}
h1 {
  font-family: normal;
  padding-right: 100%;
}
.underline {
  background: linear-gradient(135deg, #e55d87 0%, #5fc3e4 100%);
  width: 70px;
  height: 2px;
}

hr {
  display: flex;
  width: 500px;
}
</style>
