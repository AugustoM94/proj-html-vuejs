<template>
    <div class="box-image">
      <img src="../assets/images/bg4.jpg" alt="logo-history">
      <div class="content">
        <h2>Our History</h2>
        <div class="line">
            <div class="blue"></div>
            <div class="black"></div>
        </div>
        <p class="font-w">Founded by a worldwide-famous yacht racer Alfred Tannenstrick, 
            since its <br> inception back in 1977, this company has been a welcoming 
            harbor for all <br> yachting and sailing enthusiasts, from all across the US!
        </p>
        <p>We offer a real variety of professional services, from the simple yachts <br>
            chartering and corporate events, all the way to yacht repairs, upgrades
             and <br> modifications and maintenance checkups.
        </p>
        <p>With decades of professional experience in renting, repairing and transporting <br>
             just all kinds of yachts and boats under our belt – we can assure you that we <br>
             are your best choice!
        </p>
        <button class="btn">Read More</button>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'OurHistoryApp'
    // Component options
  };
  </script>
  
  <style lang="css" scoped>
  .box-image {
    position: relative;
    overflow: hidden;

  }
  
  .content {
    position: absolute;
    top: 5%;
    right:0;
    left: 50%;
    max-width: 700px;
    padding: 20px; 
  }
  

  img {
    width: 100%; 
    height: auto; 
    transform: scale(1.2);
  }
  .btn{
  color: white;
  margin-top: 20px;
  font-size: 0.9rem;
  border-radius: 5px;
  padding: 10px 20px;
  background-color: #09C2DD;
  font-family: "Poppins", Sans-serif;

}
.btn:hover{
    background-color: black;
}
.content h2{
    font-size: 3em;
    font-family: "Poppins", Sans-serif;
    font-weight: 700;
    line-height: 1.20em;
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
  width: 90%; 
  height: 1px;
  background-color: black; 
}
.content  p{
    font-size: 1.3rem;
    margin-top: 20px;
}
.font-w{
    font-weight: 700;
}
  </style>
  