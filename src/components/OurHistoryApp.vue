<template>
  <div class=" box-image">
    <div class="row">
      <div class="col-lg-6"></div>
      <div class="col-lg-6">
          <div class="content">
            <h2>Our History</h2>
            <div class="line">
              <div class="blue"></div>
              <div class="black"></div>
            </div>
            <p class="font-w">
              Founded by a worldwide-famous yacht racer Alfred Tannenstrick, since its
              <br /> inception back in 1977, this company has been a welcoming harbor for
              all
              <br /> yachting and sailing enthusiasts, from all across the US!
            </p>
            <p>
              We offer a real variety of professional services, from the simple yachts
              <br />
              chartering and corporate events, all the way to yacht repairs, upgrades and
              <br /> modifications and maintenance checkups.
            </p>
            <p>
              With decades of professional experience in renting, repairing and
              transporting
              <br /> just all kinds of yachts and boats under our belt – we can assure
              you that we
              <br /> are your best choice!
            </p>
            <button class="btn">Read More</button>
          </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'OurHistoryApp'
};
</script>

<style lang="css" scoped>
.box-image {
  background-image: url(../assets/images/bg4.jpg);
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  padding: 160px 0px 171px 0px;
  overflow: hidden;

  

}

.content {
  max-width: 700px;
  padding: 20px;


}


.btn {
  color: white;
  margin-top: 20px;
  font-size: 0.9rem;
  border-radius: 5px;
  padding: 10px 20px;
  background-color: #09c2dd;
  font-family: 'Poppins', sans-serif;
}

.btn:hover {
  background-color: black;
}

.content h2 {
  font-size: 3em;
  font-family: 'Poppins', sans-serif;
  font-weight: 700;
  line-height: 1.20em;
}

.line {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 30px;
}

.blue {
  width: 10%;
  height: 1px;
  background-color: #09c2dd;
}

.black {
  width: 90%;
  height: 1px;
  background-color: black;
}

.content p {
  font-size: 1.3rem;
  margin-top: 20px;
}

.font-w {
  font-weight: 700;
}
</style>
