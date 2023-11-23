<template>
    <section>
      <div class="row">
        <div class="col-lg-4">
          <a href="#"><img src="../assets/images/logo (1).png" alt="logo"></a>
          <p>Yacht rentals for people who love <br> sailing across the seas…</p>
        </div>
        <div class="col-lg-4 ">
          <!-- Seconda colonna -->
          <div class="d-flex">
            <ul class="mr-4">
              <li v-for="(menuItem, index) in menuItems.slice(0, 3)" :key="index">{{ menuItem }}</li>
            </ul>
            <ul>
              <li v-for="(menuItem, index) in menuItems.slice(3, 6)" :key="index">{{ menuItem }}</li>
            </ul>
          </div>
        </div>
        <div class="col-lg-4">
          <!-- Terza colonna -->
          <h3 class="mb-4">Newsletter</h3>
          <div class="d-flex">
            <input class="form-control mr-3" type="email" placeholder="Enter your email" v-model="email">
            <button class="btn">Subscribe</button>
          </div>
        </div>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'FooterAppUp',
    data() {
      return {
        menuItems: ["Yachts", "Services", "Reservations", "Blog", "Privacy Policy", "Terms Of Use"],
        email: '',
      }
    },
  }
  </script>
  
  <style lang="css" scoped>
  section {
    background-color: #F5F5F5;
    padding: 100px;
  }
  
  ul {
    list-style-type: none;
    margin-left: 0;
    padding: 0;
  }
  li{
    font-size: 1em;
    font-weight: 600;
    text-transform: uppercase;
    padding: 5px;
  }
  input {
    width: 100%;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    font-size: 0.8rem;
  }
  li:hover{
    color: #09c2dd;
    cursor: pointer;
  }
  .btn {
    color: white;
    font-size: 1rem;
    border-radius: 5px;
    padding: 15px 30px;
    background-color: #09c2dd;
    font-family: 'Poppins', sans-serif;
    border: 1px solid white;
    font-weight: 300;
    
}
.btn:hover{
    cursor: pointer;
}
  .mb-4 {
    margin-bottom: 1rem;
  }
  </style>
  