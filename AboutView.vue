<template>
  <div class="about-background-container" id="top" >
    <div class="container">
        <div class="navbar navbar-expand-lg w-100 mb-5  ">
            <div class="container">
              <a class="navbar-brand" href="#">
                <img src="../assets/img/meba-red.png" class="logo" alt="">
              </a>
              <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
              </button>
            
              <div class="collapse navbar-collapse nav-links " id="navbarNav">
                <ul class="navbar-nav link-list  ">
                  <li class="nav-item">
                    <RouterLink to="/"  class="nav-link " aria-current="page">Home</RouterLink>
                  </li>
                  <li class="nav-item">
                    <RouterLink to="/services" class="nav-link ">Services</RouterLink>
                  </li>
                  <li class="nav-item">
                    <RouterLink to="/about" class="nav-link active">About</RouterLink>
                  </li>
                  <li class="nav-item">
                    <RouterLink to="/contact" class="nav-link  ">Contact</RouterLink>
                    <a  href="/" > </a>
                  </li>
                </ul>
              </div>
            </div>
        </div>
          <div class=" head-title px-3 px-md-0 my-5 ">
            <div class="d-flex" > <span class="first-line mt-5 mb-4 " ></span></div>
            <h1 class="fs-1 lora ">About Us</h1>
            <!-- <p class=" head-paragraph py-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda optio id animi natus cupiditate nostrum ipsum sit molestias dolorum incidunt?</p> -->
            <!-- <a href="#"><button class="head-btn "> READ MORE</button></a> -->
          </div>
    </div>
    
    </div>
    <section class="hero ">
        <section class="container mt-5">
          <hr>
          <div class="row gap-3 p-3 my-5 ">
                <div class="col-md-5 col-12 p-3 border-end ">
                    <h6 class="section-title mb-3  fs-3"> Our Mission</h6>
                    <p class="section-paragraph fs-5">{{store.database.mission}}</p>
                    <!-- <hr class="vertical-line"> -->
                </div>
                <div class="col-md-6 col-12 p-3 section-paragraph" style="margin-top: 6rem;">
                    <h6 class="section-title mb-3  fs-3"> Corporate Values & Principles</h6>
                    <ol class="fs-5 px-3" style="text-align: justify;" >
                      <li>Apply high professional and ethical standards.</li>
                      <li>Provide creative and innovative solutions that fulfill clients’ needs and achieve their corporate and personal goals.</li>
                      
                      <li>Establish mutually beneficial business relationships.</li>
                    </ol>
                    <!-- <RouterLink to="/about" class=" "><button class="hero-btn "> READ MORE</button></RouterLink>      -->        
              </div> 
            </div>
          <hr>
            <div class="row   my-5 ">
                <div class="col-md-5 col-12  ">
                    <img src="../assets/img/fouad.png" class=" ms-5 px-5 fouad border-end" alt="">
                    <!-- <hr class="vertical-line"> -->
                </div>
                <div class="col-md-5 col-12   ">
                    <h1 class="section-paragraph fs-3 supername lora">{{store.database.superName}}</h1>
                    <h6 class="section-title  fs-5"> {{store.database.superTitle}}</h6>
                    <!-- <h5 class=" work section-paragraph">{{store.database.superHeading}}</h5> -->
                    <p class="section-paragraph text-justify fs-6 w-100">Served since 1987, as the leader of several
private businesses. Member of numerous advisory boards. Distinguished lecturer who holds a
doctorate in business marketing. <br>
Teaches MBA courses at prominent universities.
Was appointed multiple times Dean and Vice-
President, served on numerous university
councils.</p>
                    <!-- <a href="#"><button class="hero-btn "> READ MORE</button></a> -->
                </div>
            </div>
            <hr>
            </section>
            <!-- <section class="  quote-bg">
              <div class=" quote container my-5  ">
                <h1 class=" fs-1 lora mt-5 "><i class="bi bi-quote quote-icon"></i></h1>
                <h1 class=" fs-1 lora text-light" style="width: 60%;">We provide personalised solutions that are tailored to the unique needs of each of our clients.</h1>
                <h6 class="text-light mb-5 " style="width: 60%;">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut elit tellus, luctus nec ullamcorper mattis, pulvinar.</h6> 
              </div>
            </section> -->
            <section class="container">
              <div class="row p-3 my-5 ">
                <div class="col-md-6 col-12 ps-3 border-end ">
                  <img src="../assets/img/english-hat.jpg"  style="width: 100%; height: 260px;" alt="">
                </div>
                <div class="col-md-6 col-12 ps-3 mt-3  ">
                    <!-- <h6 class="section-title mb-3  fs-5"> Our Team</h6> -->
                    <span class="text-light fs-1 fw-bolder lora ">Meet the squad</span>
                    <hr class="text-light"> 
                </div>
                
              </div>
              <div class="row  my-5 lora ">
                <div class="col-md-3 col-12 p-2 img-pot border shadow">
                  <center><div class="image-container mb-2"><img src="../assets/img/margeurite.jpg"  alt=""></div></center>
                  <div class="person-title lora fs-4 ">{{store.database.memberOneName}}</div>
                  <h6 class="fs-5 person-title text-light">{{store.database.memberOneTitle}}</h6>
                  <p class=" person-title ">{{store.database.memberOneBio}}</p>
                </div>
                
                <div class="col-md-3 col-12 p-2 img-pot border-end shadow">
                  <center><div class="image-container mb-2"><img src="../assets/img/Reem.png"  alt=""></div></center>
                      <div class=" person-title lora fs-4"> {{store.database.memberTwoName}}</div>
                      <h6 class="fs-5 text-light ">{{store.database.memberTwoTitle}}</h6>
                      <p class=" person-title">{{store.database.memberTwoBio}}</p>
                </div>
                <div class="col-md-3 col-12 p-2 img-pot border shadow">
                  <center><div class="image-container mb-2"><img src="../assets/img/hrair.jpg"  alt=""></div></center>
                    <div class=" person-title lora fs-4">{{store.database.memberThreeName}}</div>
                    <h6 class="fs-5 text-light">{{store.database.memberThreeTitle}}</h6>
                    <p class=" person-title ">{{store.database.memberThreeBio}}</p>
                </div>
                <div class="col-md-3 col-12 p-2 img-pot border shadow">
                  <center><div class="image-container mb-2"><img src="../assets/img/Bassam.png"  alt=""></div></center>
                    <div class="person-title lora fs-3">{{store.database.memberFourName}}</div>
                    <h6 class="fs-5 text-light">{{store.database.memberFourTitle}}</h6>
                    <p class=" person-title ">{{store.database.memberFourBio}}</p>
                </div>
                
              </div>
            </section>
    </section>
    <footer class="bg-light shadow-sm down ">
      <div class="container footer ">
        <div class="row  py-3  ">
          <div class="col-md-3 col-12 py-3  d-flex justify-content-md-start justify-content-center">
              <ul >
                <li class="footer-lists"><RouterLink to="/services" class="footer-link">Marketing Audit</RouterLink></li>
                <li class="footer-lists"><RouterLink to="/services" class="footer-link">Restructuring & Reengineering</RouterLink></li>
                <li class="footer-lists"><RouterLink to="/services" class="footer-link">Strategic Planning</RouterLink></li>
                <li class="footer-lists"><RouterLink to="/services" class="footer-link">Coaching for Executives</RouterLink></li>
                <li class="footer-lists"><RouterLink to="/services" class="footer-link">SOPs & Governance</RouterLink></li>
                <li class="footer-lists"><RouterLink to="/services" class="footer-link">Education Management & Learning</RouterLink></li>
                <li class="footer-lists"><RouterLink to="/services" style=" margin-left: -3px;" class="footer-link">Training & Workshop</RouterLink></li>
              </ul>
              <!-- <hr class="vertical-line"> --> 
          </div>
          <div class="col-md-7 col-12 py-3 footer-mid ">
            <h4 class=" service-title py-2 hand fs-5 ">“Don’t dwell on what went wrong. Instead, focus on what to do next. Spend your energies on moving forward toward finding the answer</h4>
            <h6 class=" service-title hand fs-6 author ">Denis Waitley</h6>
            <a :href="'tel:'+store.database.number" class=" fs-4 phone ">{{store.database.number}}</a>
            <a :href="'mailto:'+store.database.email" class=" fs-4 footer-link">{{store.database.email}}</a>
          </div>
          <div class="col-md-2 col-12 py-3  d-flex justify-content-md-end justify-content-center">
            <ul>
              <li class="footer-lists"><RouterLink to="/" class="footer-link fs-5">Home</RouterLink></li>
              <li class="footer-lists"><RouterLink to="/about" class="footer-link fs-5">About</RouterLink></li>
              <li class="footer-lists"><RouterLink to="/services" class="footer-link fs-5">Services</RouterLink></li>
              <li class="footer-lists"><RouterLink to="/contact" class="footer-link fs-5">Contact Us</RouterLink></li>
            </ul>
            <!-- <hr class="vertical-line"> --> 
        </div>
        </div>
      </div>
      <hr>
      <div class="row  py-3 ">
        <section class="d-flex  justify-content-center  gap-4 bg-light">
          <a :href="store.database.linkedIn"><i class="bi bi-linkedin phone fs-3"></i></a>
        </section>
      </div>
    </footer>
</template>

<script >
import store from '../store.js'
export default{
  data(){
    return{
      store
      
    }
  }
}
</script>

