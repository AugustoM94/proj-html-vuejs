<template>
  <div class="box-image">
    <div class="content">
      <h2>Yacht Charters, Repairs <br> & Transportation, US-wide!</h2>
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
  background-image: url(../assets/images/bg5.jpg);
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}

.content {
  text-align: center;
}

.btn {
  color: white;
  margin-top: 20px;
  font-size: 0.9rem;
  border-radius: 5px;
  padding: 15px 30px;
  background-color: #09C2DD;
  font-family: "Poppins", sans-serif;
}

.btn:hover {
  background-color: black;
}

.content h2 {
  color: white;
  font-size: 5em;
  font-family: "Poppins", sans-serif;
  font-weight: 700;
  letter-spacing: 3px;
}
</style>
