<template>
    <div class="service-background-container" id="top">
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
                <ul class="navbar-nav link-list ">
                  <li class="nav-item">
                    <RouterLink to="/"  class="nav-link " aria-current="page">Home</RouterLink>
                  </li>
                  <li class="nav-item">
                    <RouterLink to="/services" class="nav-link active">Services</RouterLink>
                  </li>
                  <li class="nav-item">
                    <RouterLink to="/about" class="nav-link ">About</RouterLink>
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
            <h1 class="fs-1 lora">Our Services</h1>
            <!-- <p class=" head-paragraph py-3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda optio id animi natus cupiditate nostrum ipsum sit molestias dolorum incidunt?</p> -->
            <!-- <a href="#"><button class="head-btn "> READ MORE</button></a> -->
          </div>
    </div>
    
    </div>
    <section class="hero ">
        <section class="container mt-5">
          <hr>
            <div class="row  my-5 ">
                <div class="col-md-3 p-3 col-12  ">
                    <img src="../assets/img/marketing.png" style="height: 10rem;" class="w-100 h-90" alt="">
                    <h6 class="section-title mb-2 mt-2  "> 01</h6>
                    <H1 class="section-paragraph fs-2 lora">Marketing Audit </H1>
                    <hr class="">
                </div>
                <div class="col-md-3 col-12 p-3  ">
                    <h5 class=" work section-paragraph">{{store.database.service_1heading}}</h5>
                    <p class="section-paragraph">{{store.database.service_1par}}</p>
                    <!-- <a href="#"><button class="hero-btn "> READ MORE</button></a> -->
                </div>
                <div class="col-md-3 p-3 col-12  ">
                    
                    <h6 class="section-title mb-2 mt-2  "> 02</h6>
                    <H1 class="section-paragraph fs-2 lora">Restructuring & Reengineering </H1>
                    <img src="../assets/img/reingeneering.jpg" class="w-100 h-90" alt="">
                    <hr class="">
                </div>
                <div class="col-md-3 col-12 p-3  ">
                    <h5 class=" work section-paragraph">{{store.database.service_2heading}}</h5>
                    <p class="section-paragraph">{{store.database.service_2par}}</p>
                    <!-- <a href="#"><button class="hero-btn "> READ MORE</button></a> -->
                </div>
                <hr>
                <div class="col-md-3 p-3 col-12  ">
                    <img src="../assets/img/planning.jpg" class="w-100 h-90" alt="">
                    <h6 class="section-title mb-2 mt-2  "> 03</h6>
                    <H1 class="section-paragraph fs-2 lora">Strategic Planning</H1>
                    <hr class="">
                </div>
                <div class="col-md-3 col-12 p-3  ">
                    <h5 class=" work section-paragraph">{{store.database.service_3heading}}</h5>
                    <p class="section-paragraph">{{store.database.service_3par}}</p>
                    <!-- <a href="#"><button class="hero-btn "> READ MORE</button></a> -->
                </div>
                <div class="col-md-3 p-3 col-12  ">
                    <h6 class="section-title mb-2 mt-2  "> 04</h6>
                    <H1 class="section-paragraph fs-2 lora">Coaching for Executives  </H1>
                    <img src="../assets/img/coaching.jpg" style="height: 10rem;" class="w-100 h-90" alt="">
                    <hr class="">
                </div>
                <div class="col-md-3 col-12 p-3  ">
                    <h5 class=" work section-paragraph">{{store.database.service_4heading}}</h5>
                    <p class="section-paragraph">{{store.database.service_4par}}</p>
                    <!-- <a href="#"><button class="hero-btn "> READ MORE</button></a> -->
                </div>
                <hr>
                <div class="col-md-3 p-3 col-12  ">
                    <img src="../assets/img/SOP.jpg" style="height: 10rem;" class="w-100 h-90" alt="">
                    <h6 class="section-title mb-2 mt-2  "> 05</h6>
                    <H1 class="section-paragraph fs-2 lora">Stantad Operation Procedures <br>SOPs </H1>
                    <hr class="">
                </div>
                <div class="col-md-3 col-12 p-3  ">
                    <h5 class=" work section-paragraph">{{store.database.service_5heading}}</h5>
                    <p class="section-paragraph">{{store.database.service_5par}}</p>
                    <!-- <a href="#"><button class="hero-btn "> READ MORE</button></a> -->
                </div>
                <div class="col-md-3 p-3 col-12  ">
                    <img src="../assets/img/education.jpg" class="w-100 h-90" alt="">
                    <h6 class="section-title mb-2 mt-2  "> 06</h6>
                    <H1 class="section-paragraph fs-2 lora">Education Management & Learning </H1>
                    <hr class="">
                </div>
                <div class="col-md-3 col-12 p-3  ">
                    <h5 class=" work section-paragraph">{{store.database.service_6heading}}</h5>
                    <p class="section-paragraph">{{store.database.service_6par}}</p>
                    <!-- <a href="#"><button class="hero-btn "> READ MORE</button></a> -->
                </div>
                <hr>
                <div class="col-md-3 p-3 col-12  ">
                    <img src="../assets/img/training.jpg" class="w-100 h-90" alt="">
                    <h6 class="section-title mb-2 mt-2  "> 07</h6>
                    <H1 class="section-paragraph fs-2 lora">Training & Workshop </H1>
                    <hr class="">
                </div>
                <div class="col-md-8 col-12 align-items-center  d-flex flex-column ">
                  <h2 class="section-paragraph lora"> Training Topics</h2>
                  <h5 class=" work section-paragraph"> A broad range of well-designed case-based topics. <br><br> Topics can also be customized depending on the client’s requirements.</h5>
                   <!-- <h6 class="section-title work text- center" >All topics are case-based and are adapted to the client’s type of business and needs. Therefore, MEBA’s workshop bouquet is composed of the following topics:</h6> -->
                   <button class="btn hero-btn" type="button" data-bs-toggle="collapse" data-bs-target="#collapseExample" aria-expanded="false" aria-controls="collapseExample">READ MORE</button>
                   <ul class="border-light">
                    <li v-for=" t in store.database.services"  id="collapseExample" class="collapse section-paragraph fs-5 topic work">{{t.TOPIC}}</li>
                  </ul>
                </div> 
                
                <hr>
               
                <!-- <div class=" align-items-center d-flex justify-content-center section-paragraph work mt-4  fs-3">
                  <div class="text-center ">
                    {{store.database.traininReq}}
                  </div>
                  
                </div> -->
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