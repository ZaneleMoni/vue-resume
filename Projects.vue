<template>
  <hr />
  <div id="project">
      <h1>Projects</h1>
    <div class="underline"></div>
 
  <div id="projy" v-for="project of projects" :key="project.id">
<div class="card">
    <img :src="project.img_url" alt="">
    <p>{{project.title}}</p>
    <p>Github links</p>
</div>
  </div>
    
  </div>
</template>

<script>
export default {
  props: ["id"],
  data() {
    return {
      projects: [  {
      id: 1,
      img_url: "https://i.postimg.cc/GpSmqxQP/BMI.png",
      title: "BMI",
      details: "lorem10"
    },
    {
    id: 2,
      img_url: "https://i.postimg.cc/tgFqyGtT/timerproject.png",
     title: "Timer Game",
      details: "lorem"
    },
    {
    id: 3,
      img_url: "https://i.postimg.cc/nzmWjnw8/e-commerce.png",
     title :"E-commerce",
      details: "lorem"
    },
    {
    id: 4,
      img_url: "https://i.postimg.cc/QttWMM6m/helicopter.png",
     title :"Helicopter",
      details: "lorem"
    },

    {
    id: 5,
      img_url: "https://i.postimg.cc/WbsJHXVg/calculator.png",
     title: "Calculator",
      details: "lorem"
    },
  ],
    };
  },
  mounted() {
    fetch("http://localhost:3000/projects")
      .then((res) => res.json())
      .then((data) => (this.project = data))
      .catch((err) => console.log(err.message));
  },
};
</script>

<style scoped>
h1 {
  font-family: normal;
  padding-right: 100%;
 
}
.underline{
  background: linear-gradient(135deg, #e55d87 0%, #5fc3e4 100%);
  width: 70px;
  height: 2px;

}
img{
  height: 100px;
  width: 100px;
}
hr {
  display: flex;
  width: 500px;
}
#project {
  padding-left: 250px;
}
</style>
