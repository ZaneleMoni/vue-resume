<template>
    <!-- <div class="nav" id="myNav">

           <a href="#app"  >Home
 
</a>
       <a href="#about" class="navbar">About
  
</a>
    <a href="#project" class="navbar">Project
</a>
<a  href="#skill" class="navbar">Skills
</a>
<a href="#testimonial" class="navbar">Testimonials
</a>
    <a href="#contact" class="navbar">Contact
</a>

    </div> -->
    <div class="nav" id="MyNav">
    <nav class="navbar navbar-light bg-white fixed-top" style="color: black;">
  <div id="openNav" class="container-fluid"> 
    <a class="navbar-brand" href="#" style="color: white;"> 𝐍.𝐌 </a><br>
     <!-- <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar">
      <span class="navbar-toggler-icon"></span>
       </button> -->
    <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
      <div class="offcanvas-header">
        <h5 class="offcanvas-title" id="offcanvasNavbarLabel"></h5>
           </div>
      <div class="offcanvas-body">
        <ul class="navbar-nav justify-content-end flex-grow-1 pe-3">
            <span class="material-icons-round">
              
            <a class="nav-link" href="#app" ><i class=" fa fa-home"></i>Home</a>
            <a class="nav-link" href="#about"> <i class=" 	fa fa-info-circle"></i>About</a>
            <a class="nav-link" href="#resume" ><i class=" 	fa fa-mortar-board"></i>Resume</a>
            <a class="nav-link" href="#skill"> <i class=" 	fa fa-pie-chart"></i>Skills</a>
            <a class="nav-link" href="#project"><i class=" fa fa-tasks"></i>Projects</a>
            <a class="nav-link" href="#testimonial"><i class=" fa fa-group"></i>Testimonials</a>
            <a class="nav-link" href="#contact2"><i class=" 	fa fa-phone"></i>Contact</a>
       </span>
        </ul>
      </div>
    </div>
  </div>
</nav>
</div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
.nav{
  background: rgb(29, 29, 29);
  padding: 10px;
  text-align: center;
  overflow: hidden;
  text-align: center;
  margin: 0;
  position: fixed;
  height: 100%;
  width:200px;
  /* opacity: 0.7; */
}
.nav a {
  float: left;
  display: block;
  color: #eef8f8;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}
.nav a:hover {
  background-color: rgb(5, 5, 5);
  color: rgb(114, 83, 201);

}
.nav a.active {
  background-color: #b5a9bb;
  color: white;
 
}
 @media screen 
 and (device-width: 480px)
 and (device-height: 800px)
 { 
   
   @media screen and (min-width: none)  
   and (max-width: 1200px){}
 }
 
</style>