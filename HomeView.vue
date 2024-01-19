
<template>
  <main>
    <section v-if="store.spiner" class="spinner bg-light w-100 h-100 position-fixed">
      <div>
        <div class="spinner-grow text-secondary" role="status">
        <span class="visually-hidden">Loading...</span>
      </div>
      </div>
    </section>
    <div class="background-container"  >
    <div class="container">
        <div class="navbar navbar-expand-lg w-100 mb-5  " id="top">
            <div class="container">
              <a class="navbar-brand" href="#">
                <img src="../assets/img/meba-red.png" class="logo" alt="">
                <!-- <span class="MEBA lora"> Middle-East Business Advisors</span> -->
              </a>
              <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
              </button>
            
              <div class="collapse navbar-collapse nav-links " id="navbarNav">
                <ul class="navbar-nav link-list">
                  <li class="nav-item">
                    <RouterLink to="/"  class="nav-link active" aria-current="page">Home</RouterLink>
                  </li>
                  <li class="nav-item">
                    <RouterLink to="/services" class="nav-link ">Services</RouterLink>
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
            
            <div class="d-flex" > 
              <span class="first-line mt-5 mb-4 " ></span></div>
              <h1 class="fs-2 lora">{{store.database.title}}</h1>
              
                
            
            <!-- <p class=" head-paragraph py-3 work fst-italic fs-4">{{store.database.heading}}</p> -->
          </div>
    </div>
    
    </div>
    <section class="hero mb-5">
        <section class="container mt-5">
          <hr>
            <div class="row gap-3 p-3 my-5 ">
                <div class="col-md-5 col-12 p-3 border-end ">
                    <h6 class="section-title mb-3  fs-3"> About Us</h6>
                    <hr class="text-light">
                    <p class="section-paragraph fs-5">{{store.database.about}} </p>
                    <RouterLink to="/about" class=" "><button class="hero-btn "> READ MORE</button></RouterLink>                

                    <!-- <hr class="vertical-line"> -->
                </div>
                <div class="col-md-6 col-12 p-3  " style="margin-top: 6rem; text-align: justify;">
                    <h6 class="section-title mb-3  fs-3"> Why Choose Us </h6>
                    <hr class="text-light">
                    <!-- <p class="section-paragraph fs-4 lora">{{store.database.wwd_heading}}</p> -->
                    <p class="section-paragraph fs-5">{{store.database.wwd_paragraph}}</p>
                    <img src="../assets/img/chess.jpg" style="width: 32.5rem;height: 190px;" class=" ">

              </div>
              </div>
              
            <hr>
            <div class="row gap-3 p-3 my-5 services-row ">
              <div class="col-md-5 col-12 p-3 border-end">
                  <h6 class=" mb-3 text-light fs-3"> Our Services</h6>
                  <hr class="text-light ">
                  <h6 class=" fs-5 mt-4 text-light fs-4 work w-100 " style="text-align: left;" >{{store.database.services_p}}</h6>
                  <!-- <p class="section-paragraph fs-2 fw-bolder lora ">“Don’t dwell on what went wrong. Instead, focus on what to do next. Spend your energies on moving forward toward finding the answer.”<br>Denis Waitley</p> -->
                  <!-- <hr class="vertical-line"> --> 
              </div>
              <div class="col-md-5 col-12 p-3 ">
                  
                  
                  <!-- <hr class="vertical-line"> --> 
              </div>
            </div>
            <div class="row gap-4 p-3 ms-3 my-5 lora ">
              <div class="col-md-2 col-12 p-3 mb-5 service-pot" >
                <RouterLink to="/services">
                  <div class="card ">
                    <img src="../assets/img/marketing.png" style="height: 9rem;" class="card-img-top " alt="...">
                    <div class="card-body">
                    <h5 class="service-title  fw-bolder">Marketing <br> Audit</h5>
                    <br>
                    </div>
                  </div>
                </RouterLink>
              </div>
              <span class="chain-line  " ></span>
              <div class="col-md-2 col-12 p-3   service-pot  ">
                <RouterLink to="/services"> <div class="card card-hover" >
                  <img src="../assets/img/reingeneering.jpg" style="height: 9rem;" class="card-img-top " alt="...">
                  <div class="card-body">
                    <h5 class="service-title fs- fw-bolder">Restructuring & Reengineering</h5>
                    <br>
                  </div>
                </div></RouterLink>
              </div>
              <span class="chain-line  " ></span>
              <div class="col-md-2 col-12 p-3   service-pot ">
                <RouterLink to="/services">
                  <div class="card card-hover" >
                    <img src="../assets/img/planning.jpg" class="card-img-top " style="height: 9rem;" alt="...">
                    <div class="card-body">
                      <h5 class="service-title fs- fw-bolder">Strategic Planning</h5>
                      <br>
                  </div>
                </div>
                </RouterLink>
              </div>
              <span class="chain-line  " ></span>
              <div class="col-md-2 col-12 p-3   service-pot">
                <RouterLink to="/services">
                  <div class="card card-hover" >
                    <img src="../assets/img/coaching.jpg" style="height: 9rem;" class="card-img-top " alt="...">
                    <div class="card-body">
                      <h5 class="service-title fs- fw-bolder">Coaching for Executives</h5>
                      <br>
                    </div>
                  </div>
                </RouterLink>
                
               </div>
               <div class="col-md-1 col-12 p-3 ms-md-5   service-pot">
                <RouterLink to="/services">
                  <div class="card card-hover " >
                  <img src="../assets/img/SOP.jpg" style="height: 7.5rem;" class="card-img-top " alt="...">
                  <div class="card-body">
                    <h5 class="service-title fs- fw-bolder">Stantad Operation Procedures <br>SOPs</h5>
                    <br>
                  </div>
                </div>
                </RouterLink>
                
               </div>
               <span class="chain-line  " ></span>
               <div class="col-md-2 col-12 p-3   service-pot">
                <RouterLink to="/services">
                  <div class="card card-hover" >
                  <img src="../assets/img/education.jpg" style="height: 9rem;" class="card-img-top " alt="...">
                  <div class="card-body">
                    <h5 class="service-title f fw-bolder">Education Management & Learning</h5>
                  </div>
                </div>
                </RouterLink>
                
               </div>
               <span class="chain-line  " ></span>
               <div class="col-md-2 col-12 p-3   service-pot">
                <RouterLink to="/services">
                  <div class="card card-hover " >
                   <img src="../assets/img/training.jpg" style="height: 9rem;" class="card-img-top" alt="...">
                  <div class="card-body">
                    <h5 class="service-title  fw-bolder">Training & Workshop</h5>
                    <br>
                  </div>
                </div>
                </RouterLink>
               </div>
               <span class="chain-line  " ></span>
               <div class="col-md-2 col-12 p-3   service-pot">
                <RouterLink to="/services">
                  <div class="card card-hover" style="height: 9rem;"  >
                   <img src="../assets/img/button.png" style="height: 9rem;" class="card-img-top" alt="...">
                  <div class="card-body">
                    <h5 class="service-title  fw-bolder">Click to know more about our services</h5>
                    <br>
                  </div>
                </div>
                </RouterLink>
               </div>
               <span class="final-line  " ></span>
               </div>
               

               
      

              
              
           
        </section>
          <!-- <div class="container">
            <div class="row gap-3 p-3 my-5 ">
              <hr class="text-light">
              <div class="col-md-4 col-12 p-3 ">
                  <h6 class="section-title mb-3 text-light fs-4"> Projects</h6>
                  <p class="section-paragraph fs-1 text-light fw-bolder lora ">Featured Case Studies</p>
                  <hr class="vertical-line"> 
              </div>
            </div>
            <div class="row   mb-5 px-3 ">
              <hr class="text-light">
              <div class="col-md-6 col-12  text-end ">
              <hr class="vertical-line text-light">   
              </div>
              <div class="col-md-5 col-12  ">
                <div class="  text-light ">
                  <h1 class="section-title text-light fw-bolder lora"> {{store.database.comp_1}}</h1>
                  <p class="section-paragraph fs-5 text-light  ">{{store.database.comp_1p}}</p>
                </div>
                <div class=" p-1 text-light">
                  <hr class="text-start fw-bold">
                  <h1 class="section-title text-light fw-bolder lora"> {{store.database.comp_2}}</h1>
                  <p class="section-paragraph fs-4 text-light  ">{{store.database.comp_2p}}</p>
                </div>
                <div class=" p-1 text-light">
                  <hr>
                  <h1 class="section-title text-light fw-bolder lora"> {{store.database.comp_3}}l</h1>
                  <p class="section-paragraph fs-4 text-light  ">{{store.database.comp_3p}}</p>
                </div>
                 <hr class="vertical-line">  
              </div>
            </div>

          </div> -->
          
        </section>
         <section class="case-study figures"> 
          <div class="container">
            <div class="row  p-3 my-5 ">
              <hr class="text-light">
              <div class="col-md-5 col-12 p-3 border-end">
                  <!-- <h6 class="section-title mb-3 text-light fs-4"> Projects</h6> -->
                  <p class="section-paragraph fs-1 text-light fw-bolder lora ">Target Customers</p>
                  <img src="../assets/img/customer.jpg"  style="width: 25rem; height: 260px;" alt="">
                  <hr class="text-light">
                 
              </div>
            <!-- </div> -->
            <!-- <div class="row   mb-5 px-3 "> -->
              <div class="col-md-5 justify-content-end col-12" style="width: 40rem;">
                <div class="  text-light ">
                  <h1 class="section-paragraph  fw-bolder fs-3 lora"> Private orginizations</h1>
                </div>
                <div class=" p-1 text-light">
                  <hr class="text-start fw-bold">
                  <h1 class="section-paragraph fw-bolder fs-3 lora"> Public sector</h1>
                </div>
                <div class=" p-1 text-light">
                  <hr>
                  <h1 class="section-paragraph fw-bolder fs-3 lora"> NPOS & NGOS</h1>
                </div>
                <div class=" p-1 text-light">
                  <hr>
                  <h1 class="section-paragraph fw-bolder fs-3 lora"> Higher education institutions and schools.</h1>
                </div>
                <div class=" p-1 text-light">
                  <hr>
                  <h1 class="section-paragraph fw-bolder  fs-3 lora"> Individuals</h1>
                </div>
              </div>
            </div>

          </div>
          
        </section> 
        <!-- <section>
          <div class="container">
            <div class="row  p-3 my-5 figures ">
              <hr>
              <div class="col-md-6 col-12   ">
                  <h6 class="section-title mb-3  fs-3"> Target Markets</h6>
                   <img src="../assets/img/target.jpg" class=" w-100 my-5 " style="height: 16rem;" alt="..."> -->
                  <!-- <p class="section-paragraph fs-1 fw-bolder lora ">Elevating Experiences, Tailored for You.</p> -->
                  <!-- <hr class="vertical-line"> 
              </div>
              <div class="col-md-6 col-12  ">
                <div class="d-flex justify-content-center align-items-center justify-content-center shadow w-100 h-50 px-4  service-pot">
                  <span class="section-paragraph fs-5 work">Private and public organizations</span>
                </div>
                <div class="d-flex justify-content-center align-items-center justify-content-center shadow w-100 h-50 px-4  service-pot">
                  <span class="section-paragraph fs-5 work">NPOs and NGOs</span>
                </div>
                <div class="d-flex justify-content-center align-items-center justify-content-center shadow w-100 h-50 px-4  service-pot">
                  <span class="section-paragraph fs-5 work">Higher education institutions and schools.</span>
                </div>
                <div class="d-flex justify-content-center align-items-center justify-content-center shadow w-100 h-50 px-4  service-pot">
                  <span class="section-paragraph fs-5 work">Individuals.</span>
                </div>
              </div>
          </div>
          </div>
        </section> -->
   
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
  </main>
</template>

<script >
import store from '../store.js'
export default{
  data(){
    return{
      store,
      
      
    }
  }
}
</script>
