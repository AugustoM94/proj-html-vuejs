<template>
   <div class="box-image">
      <img src="../assets/images/bg5.jpg" alt="logo-history">
      <div class="content">
        <h2>Yacht Charters, Repairs <br> & Transportation, US-wide!
        </h2>
        <button class="btn">More Details</button>
      </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="css" scoped>
.box-image {
    position: relative;
    overflow: hidden;

  }
  
  .content {
    min-width: 1300px;
    position: absolute;
    top: 30%;
    right:0;
    left: 0;
    max-width: 700px;
    text-align: center;

  }
  

  img {
    width: 100%; 
    height: auto; 
    transform: scale(1.3);
  }
  .btn{
  color: white;
  margin-top: 20px;
  font-size: 0.9rem;
  border-radius: 5px;
  padding: 15px 30px;
  background-color: #09C2DD;
  font-family: "Poppins", Sans-serif;

}
.btn:hover{
    background-color: black;
}
.content h2{
    color: white;
    font-size: 5.8em;
    font-family: "Poppins", Sans-serif;
    font-weight: 700;
    letter-spacing: 3px;
    }

</style>