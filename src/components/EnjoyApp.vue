<template>
    <div class=" box-image">
      <div class="row">
        <div class="col-lg-6">
            <div class="content">
              <h2>Enjoy</h2>
              <h3>World Rally 2017-19</h3>
              <p>
                Explore some of the most beautiful regions of the world. Make your dreams
                 come true and join the Yachtec World Rally 2017-19.
                </p>
                <button class="btn">More Details</button>
              </div>
        </div>
        <div class="col-lg-6">
            </div>
        </div>
      </div>
  </template>
  <script>
  export default {
    name: 'EnjoyApp'
  };
  </script>
  
  <style lang="css" scoped>
  .box-image {
    background-image: url(../assets/images/bg7.jpg);
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    padding: 260px 0px 171px 0px;
    overflow: hidden;
  
    
  
  }
  
  .content {
    max-width: 700px;
    padding: 20px;
    color: white;
  
  
  }
  
  
  .btn {
    color: white;
    margin-top: 20px;
    font-size: 0.9rem;
    border-radius: 5px;
    padding: 20px 40px;
    background-color: #09c2dd;
    font-family: 'Poppins', sans-serif;
    font-weight: 700;
  }
  
  .btn:hover {
    background-color: black;
  }
  
  .content h2 {
    font-size: 125px;
    font-family: 'Poppins', sans-serif;
    line-height: 1.20em;
    font-weight: 700;
    text-transform: uppercase;
  }
  
  .content h3 {
    font-size: 65px;
    font-family: 'Poppins', sans-serif;
    line-height: 1.20em;
    font-weight: 300;
    text-transform: uppercase;
  }
  .content p {
    font-size: 1.1rem;
    margin-top: 20px;
    font-weight: 300;
  }
  
  
  </style>
  