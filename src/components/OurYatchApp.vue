<template>
    <div class="bg-yachts">
        <div class="container">
            <h2 class="text-center">Our Yachts</h2>
            <div class="line"></div>
            <div class="row">
                <div class="col-lg-3 ">
                    <img  src="../assets/images/services-1.jpg" alt="logo-1">
                    <div class=" icon-hover text-center ">
                        <a href="#"><i class="fas fa-anchor"></i></a>
                        <h3 class="text-white">Express</h3>
                        
                    </div>
                </div>
                <div class="col-lg-3 ">
                    <img src="../assets/images/services1.jpg" alt="logo-2">
                    <div class=" icon-hover text-center ">
                     <a href="#"><i class="fas fa-anchor"></i></a>
                      <h3 class="text-white">Cruisers</h3>
                    </div>
                </div>
                <div class="col-lg-3 ">
                    <img src="../assets/images/services2.jpg" alt="logo-3">
                    <div class=" icon-hover text-center ">
                        <a href="#"><i class="fas fa-anchor"></i></a>
                        <h3 class="text-white">Sport Cruisers</h3>
                    </div>
                </div>
                <div class="col-lg-3 ">
                    <img src="../assets/images/services3.jpg" alt="logo-4">
                    <div class="icon-hover text-center ">
                        <a href="#"><i class="fas fa-anchor"></i></a>
                        <h3 class="text-white">Flybridges</h3>
                    </div>
                </div>
            </div>

            <div class="row mt-4 ">
                <div class="col-lg-3 ">              
                          <img src="../assets/images/services4.jpg" alt="logo-5">
                          <div  class=" icon-hover text-center ">
                            <a href="#"><i class="fas fa-anchor"></i></a>
                           <h3 class="text-white">Sedan Bridges</h3>
                          </div>
                 </div>
                <div class="col-lg-3">               
                         <img src="../assets/images/services5.jpg" alt="logo-6">
                         <div class=" icon-hover text-center ">
                            <a href="#"><i class="fas fa-anchor"></i></a>
                            <h3 class="text-white">Tri-deck</h3>
                         </div>
                 </div>
                <div class="col-lg-3">                
                        <img src="../assets/images/services6.jpg" alt="logo-7">
                        <div class="icon-hover text-center ">
                            <a href="#"><i class="fas fa-anchor"></i></a>
                            <h3 class="text-white">Megayachts</h3>
                        </div>
               </div>
                <div class="col-lg-3">                   
                     <img src="../assets/images/services7.jpg" alt="logo-8">
                     <div class="icon-hover text-center ">
                        <a href="#"><i class="fas fa-anchor"></i></a>
                        <h3 class="text-white">Convertibles</h3>
                     </div>
              </div>
            </div>
       </div>
       <div class="center-btn">
                <button class="btn">View All</button>
      </div>
 </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="css" scoped>
.bg-yachts{
    background-color: #09C2DD;
}
img{
    max-width: 300px;
}
h2{
    font-size: 3em;
    color: white;
    padding:50px 0;
    font-family: "Poppins", Sans-serif;
    font-weight: 700;
}
.col-lg-3{
    position: relative;
    overflow: hidden;
    border-radius: 5%;

}
.line {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 20px;
  margin-bottom: 50px;
  width: 5%;
  height: 1px;
  background-color: white;
}
.icon-hover {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-size: 5em;
    color: #09C2DD;
    opacity: 0; 
    transition: opacity 0.3s ease-in-out, transform 0.3s ease-in-out;
    font-family: "Poppins", Sans-serif;
    font-weight: 300;

}

a{
    color: #09C2DD;

}
.col-lg-3:hover .icon-hover {
    opacity: 1; 

}
.col-lg-3:hover  {
    cursor: pointer;
} 
img:hover{
    filter: grayscale(100%);

}    

.center-btn {
    display: flex;
    justify-content: center;
    padding: 60px 0;
}

.btn {
    color: white;
    font-size: 0.9rem;
    border-radius: 5px;
    padding: 15px 30px;
    background-color: #09c2dd;
    font-family: 'Poppins', sans-serif;
    border: 1px solid white;
    font-weight: 300;
    
}
.btn:hover{
    background-color: white;
    color: black;
}
</style>