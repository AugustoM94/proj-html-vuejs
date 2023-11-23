<template>
    <div>
      <section>
          <div class="row">
            <div class="col-lg-6 d-flex">
              <ul class="d-flex justify-content-start">
                <li class="hover-effect">Zemez <span>©. All Rights Reserved.</span></li>
                <li>|</li>
                <li class="hover-effect">Privacy Policy</li>
                <li>|</li>
                <li class="hover-effect">Terms Of Use</li>
              </ul>
            </div>
            <div class="col-3"></div>
            <div class="col-lg-3 d-flex justify-content-end ">
              <div>
                <ul class="d-flex ">
                  <li>
                    <a href="#">
                      <i class="fa-brands fa-facebook"></i>
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      <i class="fa-brands fa-twitter"></i>
                    </a>
                  </li>
                  <li>
                    <a href="#">
                      <i class="fa-brands fa-instagram"></i>
                    </a>
                  </li>
                </ul>
              </div>
            </div>
          </div>
      </section>
    </div>
  </template>
  
  <script>
  export default {
    // Your component logic goes here
  };
  </script>
  
  <style lang="css" scoped>
  section {
    background-color: #222627;
    padding: 20px;
    margin: 0;
  }

  span {
    color: lightgray;
  }
  
  ul {
    list-style: none;
    margin: 0;
    padding: 0;
  }
  
  li {
    color: white;
  }
  
  a > i {
    background-color: #8B8E90;
    border-radius: 50%;
    padding: .3rem;
    font-size: 0.8rem;
    color: #222627;
    margin-right: 15px;
  }
 .hover-effect:hover {
  /* Add your hover styles here */
  cursor: pointer;
  color: #09c2dd;
}


.col-lg-6 li{
    padding: 0 10px;
    text-transform: uppercase;
    font-size: 0.8em;
}
a > i:hover{
    background-color: white;
}
  </style>
  