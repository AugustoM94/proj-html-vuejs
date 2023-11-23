<template>
      <section class="bg-white">
        <div class="container">
          <div class="row">
            <div class="col-lg-6">
                <div class="d-flex justify-content-between">
                  <div class="px-2">
                    <i class="fa-solid fa-location-dot px-2 mt-1" style="color: #09c2dd;"></i>
                    <span>7078 Richmond hwy, Alexandria, VA</span>
                  </div>
                  <div class="px-2">
                    <i class="fa-solid fa-phone px-2 mt-1" style="color: #09c2dd;"></i>
                    <span>800-2345-6789</span>
                  </div>
                </div>
            </div>
              <div class="col-lg-4"></div>
                <div class="col-lg-2">
                  <ul class="d-flex">
                    <li>
                      <a href="#">
                        <i class="fa-brands fa-facebook" style="color: #f5f6f9;"></i>
                      </a>
                    </li>
                    <li>
                      <a href="#">
                        <i class="fa-brands fa-twitter" style="color: #f5f6f9;"></i>
                      </a>
                    </li>
                    <li>
                      <a href="#">
                        <i class="fa-brands fa-instagram" style="color: #f5f6f9;"></i>
                      </a>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
      </section>
  </template>
  
  <script>
  export default {
  };
  </script>
  
  <style lang="css" scoped>

  
  span {
    color: #5E5E5E;
    font-size: 0.8rem;
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
    font-size: 0.7rem;
    color: #222627;
    margin: 0;
  }

  section {
    background-color: #222627;
    padding: 10px;
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
  
span:hover{
  color:  #09c2dd;
  cursor: pointer;
}

.col-lg-6 li{
    padding: 0 5px;
    text-transform: uppercase;
    font-size: 0.8em;
}
  </style>
  