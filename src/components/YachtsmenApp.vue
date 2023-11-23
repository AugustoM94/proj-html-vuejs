<template>
<div class="container text-center py-5">
    <h2>Yachtsmen's Blog</h2>
    <div class="line">
        <div class="black"></div>
        <div class="blue"></div>
        <div class="black"></div>
    </div>

    <div class="row">
        <div class="col-lg-4">
            <div class="card border-0" style="width: 25rem;">
                <img class="card-img-top" src="../assets/images/post1-1-570x450.jpg" alt="Card image cap">
                <div class="card-body text-center">
                    <small>December 16, 2020</small>
                    <h5 class="card-title mt-2">Is Greece a Good Choice for Yacht Sailing</h5>
                </div>
            </div>
        </div>

        <div class="col-lg-4">
            <div class="card border-0" style="width: 25rem;">
                <img class="card-img-top" src="../assets/images/post2-1-570x450.jpg" alt="Card image cap">
                <div class="card-body text-center">
                    <small>December 16, 2020</small>
                    <h5 class="card-title mt-2">Seattle Yachts and Northwest Yachts Announce Merger</h5>
                </div>
            </div>
        </div>

        <div class="col-lg-4">
            <div class="card border-0" style="width: 25rem;">
                <img class="card-img-top" src="../assets/images/post1-1-570x450.jpg" alt="Card image cap">
                <div class="card-body text-center">
                    <small>December 16, 2020</small>
                    <h5 class="card-title mt-2">Video: Superyacht ‘Project Jupiter’ Launched By Lurssen</h5>
                </div>
            </div>
        </div>
    </div>
    <button class="btn">View All Blog Posts</button>
</div>

</template>

<script>
    export default {
        
    }
</script>

<style lang="css" scoped>
.line {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 30px 0;
}
.blue {
  width: 5%; 
  height: 1px; 
  background-color:#09C2DD;
}

.black {
  width: 55%; 
  height: 1px;
  background-color: lightgrey; 
}
h2{
    font-size: 2.5em;
    color: #3A3A50;
    line-height: 1.2em;
    font-weight: 700;
    padding: 60px 0;
}
small{
    font-size: 0.7em;
}
h5{
    color: #222627;
    font-size: 1.5em;
    font-weight: 700;
    line-height: 1.5em;
}
h5:hover{
    color: #09C2DD;
    cursor: pointer;
}
.card:hover{
    cursor: pointer;
}
.btn {
    color: white;
    margin-top: 20px;
    font-size: 0.9rem;
    border-radius: 5px;
    padding: 15px 30px;
    background-color: #09c2dd;
    font-family: 'Poppins', sans-serif;
    font-weight: 700;
  }
  
  .btn:hover {
    background-color: black;
  }
</style>