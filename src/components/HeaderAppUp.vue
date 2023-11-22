<template>
    <div class=" d-flex justify-content-between  mt-2 ">
        <div class="d-flex justify-content-between ">
            <div class="px-2">
                <i class="fa-solid fa-location-dot px-2 mt-1" style="color: #09c2dd;"></i>
                <span>7078 Richmond hwy, Alexandria, VA</span>
            </div>
            <div class="px-2">
                <i class="fa-solid fa-phone px-2 mt-1" style="color: #09c2dd;"></i>
                <span>800-2345-6789</span>
            </div>
        </div>

     <div >
         <ul  class=" d-flex justify-content-between">
            <li>
                <a href="#">
                    <i class="fa-brands fa-facebook" style="color: #f5f6f9;"></i>
                </a>
                </li>
            <li>
                <a href="#">
                    <i class="fa-brands fa-twitter"  style="color: #f5f6f9;"></i>
                </a>
            </li>
            <li>
                <a href="#">
                    <i class="fa-brands fa-instagram"  style="color: #f5f6f9;"></i>
                </a>
            </li>

         </ul>
     </div>
  </div>
</template>

<script>
import '@fortawesome/fontawesome-free/css/all.css';


    export default {
        name: 'HeaderAppUp'
        
    }
</script>

<style lang="css" scoped>
a > i{
    background-color: #8B8E90;
    border-radius: 50%;
    padding: .3rem;
    font-size: 0.8rem;
}
li{
    list-style: none;
    padding: 0 10px;

}
span {
    color: #5E5E5E;
}
span:hover{
    color: #09c2dd;
    cursor: pointer;
}
</style>