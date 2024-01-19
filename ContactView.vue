<template>
    <div class="contact-background-container" id="top">
        <div class="container">
            <div class="navbar navbar-expand-lg w-100 mb-5  ">
                <div class="container">
                    <RouterLink to="/"  class="nav-link " aria-current="page">
                    <img src="../assets/img/meba-red.png" class="logo" alt="">
                  </RouterLink>
                  <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon nav-icon"></span>
                  </button>
                
                  <div class="collapse navbar-collapse nav-links " id="navbarNav">
                <ul class="navbar-nav link-list ">
                  <li class="nav-item">
                    <RouterLink to="/"  class="nav-link " aria-current="page">Home</RouterLink>
                  </li>
                  <li class="nav-item">
                    <RouterLink to="/services" class="nav-link ">Services</RouterLink>
                  </li>
                  <li class="nav-item">
                    <RouterLink to="/about" class="nav-link ">About</RouterLink>
                  </li>
                  <li class="nav-item">
                    <RouterLink to="/contact" class="nav-link  active">Contact</RouterLink>
                    <a  href="/" > </a>
                  </li>
                </ul>
              </div>
                </div>
            </div>
              <!-- <div class=" head-title px-3 px-md-0 my-5 ">
                <div class="d-flex" > <span class="first-line mt-5 mb-4 " ></span></div>
                <h1 class="fs-1 lora">Contact Us</h1>
                 <p class=" head-paragraph py-3">Cras a dictum erat. Maecenas fermentum fermentum turpis,
                     quis malesuada metus pellentesque quis. Donec semper urna lacinia justo tincidunt, ac aliquet nisi. </p>
                <a href="#"><button class="head-btn "> READ MORE</button></a> 
              </div> -->
        </div>
        
        </div>
    <section class="hero ">
        <section class="container mt-5">
          <hr>
            <div class="row my-5 ">
                <div class="col-md-6 p-3 col-12 border-end  ">
                    <hr class="">
                    <H1 class="section-paragraph fs-2 lora">Get In Touch </H1>
                    <!-- <h5 class=" work fw-lighter mt-2 fs-5 section-paragraph">We help businesses and individuals navigate the complex world of finance.</h5> -->
                    <div class="d-flex" > <span class="contact-first-line mt-2" ></span></div>
                    <div class="phone my-2 "><i class="bi bi-envelope-fill fs-5"></i> <a :href="'mailto:'+store.database.email"  class="mx-2 phone">{{store.database.email}}</a></div>
                    <div class="phone my-2"><i class="bi bi-telephone-outbound-fill fs-5"></i><a :href="'tel:'+store.database.number" class="mx-2 phone">{{store.database.number}}</a></div>
                    <div class="phone my-2 "><i class="bi bi-envelope-fill fs-5"></i> <a href="mailto:ritam.abed@yahoo.com"  class="mx-2 phone">ritam.abed@yahoo.com</a></div>
                    <div class="phone my-2"><i class="bi bi-telephone-outbound-fill fs-5"></i><a href="tel:009613226884" class="mx-2 phone">00961 3 226884</a></div>
                    <div class="phone my-2 "><i class="bi bi-envelope-fill fs-5"></i> <a href="mailto:reemnameh78@gmail.com"  class="mx-2 phone">reemnameh78@gmail.com</a></div>

                </div>
                <div class="col-md-6 col-12 p-3 mt-4 ">
                  <form @submit.prevent="sendEmail" >
                    <div class="mb-3 mt-1 d-flex">
                        <span class="form-span">
                        <label for="exampleFormControlInput1" id="name" class="form-label" required:true>Name</label>
                        <input  type="text" class="form-control" id="exampleFormControlInput1" placeholder="Name"> 
                        </span>
                        <span class="form-span ms-3 ">
                          <label for="exampleFormControlInput1" id="email" class="form-label" required:true>Email</label>
                            <input  type="email" class="form-control" id="exampleFormControlInput1" placeholder=" Email">
                            </span>
                      </div>
                      <div class="mb-3 mt-1 d-flex">
                        <span class="form-span">
                        <label for="exampleFormControlInput1" id="country" class="form-label" required:true>Country</label>
                        <input  type="text" class="form-control" id="exampleFormControlInput1" placeholder="Country"> 
                        </span>
                        <span class="form-span ms-3 ">
                          <label for="exampleFormControlInput1" id="phone" class="form-label" required:true>Phone number</label>
                            <input  type="text" class="form-control" id="exampleFormControlInput1" placeholder=" Phone number">
                            </span>
                            
                      </div>
                      <div class="mb-3">
                        <label for="exampleFormControlTextarea1" id="message" class="form-label" required:true>Message</label>
                        <textarea  v-model="store.message" class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
                      </div>
                    <button class="send-btn " type="submit"> SEND</button>
                    </form>
                    </div>
                </div>
           =
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
              <li class="footer-lists"><Router-view to="/" class="footer-link fs-5">Home</Router-view></li>
              <li class="footer-lists"><RouterLink to="/about#tpo" class="footer-link fs-5">About</RouterLink></li>
              <li class="footer-lists"><RouterLink to="/services#top" class="footer-link fs-5">Services</RouterLink></li>
              <li class="footer-lists"><RouterLink to="/contact#top" class="footer-link fs-5">Contact Us</RouterLink></li>
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
  },
  methods:{
    // send(){
    //   return `mailto: ${this.store.database.email}?subject=${this.store.subject}&body=${this.store.message}`
    // },
    sendEmail(){
  Email.send({
    Host : "smtp.elasticemail.com",
    Username : "consultmeba@gmail.com",
    Password : "7DBD5F29E392F4F693F33779E75A7B1E50F7",
    To : 'hammoudwassim837@gmail.com',
    From : "consultmeba@gmail.com",
    Subject : "This is the subject",
    Body : "And this is the body"
}).then(
  message => alert(message)
);
}
  }
}
</script>