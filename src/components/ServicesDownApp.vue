<template>
    <div class="box-image">
        <div class="container py-5">
        <h2 >Services</h2>
        <div class="line">
            <div class="black"></div>
            <div class="blue"></div>
            <div class="black"></div>
        </div>
      <div class="row">
        <div class="col-lg-4">
            <div class="mb-4">
                <span><i  class="fa-solid fa-anchor" style="color: #ffffff;"></i></span>
                <h3>Yatch Rentals</h3>
            </div>
            <div>
                <p>
                    With more than two hundred yacht and boat models on our fleet and both the East and the West coasts covered,
                     we are able to offer you the best yacht chartering options.
                </p>
            </div>
        </div>
        
        
  <div class="col-lg-4">
    <div class="mb-4">
                <span><i   class="fa-regular fa-user" style="color: #ffffff;"></i></span>
                <h3>Yatch Rentals</h3>
            </div>
            <div>
                <p>
                    On par with providing an amazing range of rentals on boats and yachts of all sizes and comfort levels, 
                    we will also gladly pick up on providing all kinds of maintenance…           
                 </p>
      </div>        
  </div>
        <div class="col-lg-4">
            <div class="mb-4">
                <span><i  class="fa-solid fa-truck-fast" style="color: #ffffff;"></i></span>
                <h3>Yatch Rentals</h3>
            </div>
            <div>
                <p>
                    Whenever any of our clients wants to try some brand new sailing destination or make a place of residence 
                    move to another water area – there comes the issue of logistics.
                </p>
      </div>       
     </div>
      </div>
      <div class="row">
        <div class="col-lg-4">
            <div class="mb-4 mt-5">
                <span><i  class="fa-regular fa-star" style="color: #ffffff;"></i></span>
                <h3>Yatch Rentals</h3>
            </div>
            <div>
                <p>
                    With decades of professional experience in renting, repairing and transporting just all kinds of 
                    yachts and boats under our belt – we can assure you that we are your best choice!   
             </p>
      </div>             
      </div>
        <div class="col-lg-4">
            <div class="mb-4 mt-5">
                <span><i   class="fa-regular fa-thumbs-up" style="color: #ffffff;"></i></span>
                <h3>Yatch Rentals</h3>
            </div>
            <div>
                <p>
                    As far as any personally-owned vehicles are concerned, whether we are talking about cars with four wheels,
                     bikes with two wheels or yachts with no wheels, owners do…
             </p>
      </div>       
      </div>
        <div class="col-lg-4">
            <div class="mb-4 mt-5">
                <span><i class="fa-solid   fa-suitcase" style="color: #ffffff;"></i></span>
                <h3>Yatch Rentals</h3>
            </div>
            <div>
                <p>
                    When it comes to organizing a corporate yacht charter of a Fortune 500 scale for a big crew of people 
                    – we will be able to make it flawless.We will exceed your expectations!
             </p>
      </div>       
        </div>
      </div>
    </div>
    </div>
  </template>
  
  <script>
  import '@fortawesome/fontawesome-free/css/all.css';

  export default {
    name: 'ServicesDownApp',
    data() {
    return {
      
};
}
}
  </script>

<style lang="css" scoped>
.box-image{
    background-image: url(../assets/images/bg6.jpg);
    width: 100%;
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    background-attachment: fixed;   

}
 h2{
    text-align: center;
    font-size: 3em;
    padding: 20px;
}
.line {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 30px 0;
}
.blue {
  width: 10%; 
  height: 1px; 
  background-color:#09C2DD;
}

.black {
  width: 45%; 
  height: 1px;
  background-color: black; 
}
i{
    font-size: 40px;
    padding: 25px;
    background-color: #09C2DD;
    border-radius: 50%;
    margin-right: 20px;


}
h3 {
    display: inline-block;
    font-weight: 700;
    font-size: 2em;
}
p{
    font-size: 1.2em;
    line-height: 1.8em;
    color: #5e5e5e;
}

</style>