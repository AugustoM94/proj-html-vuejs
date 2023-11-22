<template>
  <div class="carousel w-100 ">
    <transition name="fade">
      <img :key="currentIndex" :src="images[currentIndex]" alt="Carousel Image" @mousedown="startAutoPlay" @mouseup="stopAutoPlay" @mouseleave="stopAutoPlay" class="carousel-image" />
    </transition>

    <div class="indicators">
      <span v-for="(image, index) in images" :key="index" @click.prevent.native="goToImage(index)" :class="{ active: index === currentIndex }"></span>
    </div>

    <div v-if="currentIndex === 0" class=" overlay-menu row align-items-center mt-2 ">
      <div class="col-lg-3">
              <img src="../assets/images/logo.png" alt="logo">
        </div>
        <div class="col-lg-6 ">
            <ul  class="list-unstyled d-flex justify-content-between align-content-center mt-2 ">
                    <li>
                      <a href="#">About</a>
                    </li>
                    <li>
                      <a href="#">Services</a>
                    </li>
                      <li @mouseenter="toggleDropdown('Yachts')" class="dropdown">
                       <a href="#">Yachts</a>                            
                           <div class="dropdown-content">
                              <ul>
                                <li v-for="(submenuItem, index) in submenuItems" :key="index">                             
                                    <a :href="submenuItem.link">{{ submenuItem.label }}</a>
                                </li>                       
                              </ul>
                        </div>              
                    </li>
                    <li>
                      <a href="#">Reservations</a>
                    </li>
                    <li>
                      <a href="#">Blog</a>
                    </li>
                    <li>
                      <a href="#">Contact</a>
                    </li>
            </ul>
            
      <div class="col-lg-3 d-flex justify-content-end">
        </div>
            </div>
         <div class="col-lg-3 d-flex justify-content-end   ">    
               <i class="fa-solid fa-magnifying-glass"></i>
        </div>
        <div class="titolo"> 
                  <h1>QuickWind</h1>
                  <p>all kinds of boats, yachts characters and sailing destinations <br> for hobbyst yachtsmen and women</p> 
                  <button class="btn">Learn More</button>
        </div>
      </div>
      <div v-if="currentIndex === 1" class="overlay-menu-2 row mt-4 text-white ">
          <div class="col-lg-12 text-center">
                <h2>Flybridges, Convertibles, Expresses,<br> Sports Cruisers and more...</h2>
                <p>we've got a beautiful variety at different types of yachts...</p>
                <button class="btn">Yachts</button>
          </div>
        </div>
        <div v-if="currentIndex === 2" class="overlay-menu-3 row mt-4 text-white ">
          <div class="col-lg-12 text-center">
                <h2>Corporate yatch chartering</h2>
                <p>As far as our list of clients goes, a vast majority of those are private,hobbyst(and sometimes professional or retired professional)
                  yachtsmen and <br> women, or racers. However, when it comes to organizing a corporate yatch charter of a Fortune 500 scale for a big crew
                   of people-we will be able to make <br> it flawless!
                </p>
                <button class="btn">Yachts</button>
          </div>
        </div>
    </div>
</template>

<script>
export default {
  data() {
  return {
    images: [
      '/src/assets/images/bg1-1.jpg',
      '/src/assets/images/bg2.jpg',
      '/src/assets/images/bg3.jpg',
    ],
    currentIndex: 0,
    autoPlayInterval: null,
    zoomed: false,
    showSubmenu: false,
    submenuItems: [
      { label: 'Cruisers', link: '#' },
      { label: 'Expresses', link: '#' },
      { label: 'Sports Cruisers', link: '#' },
      { label: 'Convertibles', link: '#' },
      { label: 'Megayachts', link: '#' },
      { label: 'Tri-Deck', link: '#' },
      { label: 'Sedan Bridges', link: '#' },
      { label: 'Flybridges', link: '#' },
    ],
  };
},
  methods: {
    goToImage(index) {
      this.currentIndex = index;
      this.zoomed = false; // Resetta lo zoom quando cambia l'immagine
    },
    startAutoPlay() {
      this.changeImage(1); // Cambiare l'immagine subito quando inizia il click
    },
    stopAutoPlay() {
      // Lasciare vuoto, in quanto non vogliamo più cambiare immagini quando il click è rilasciato
    },
    changeImage(offset) {
      // Verificare che il cambio immagine non vada oltre i limiti
      const newIndex = this.currentIndex + offset;
      if (newIndex >= 0 && newIndex < this.images.length) {
        this.currentIndex = newIndex;
        this.zoomed = false; // Resettare lo zoom quando cambia l'immagine
      }
    },
    toggleDropdown(menuItem) {
      this.showSubmenu = menuItem === 'Yachts';
      
    },
  },
}
</script>
<style>
.carousel {
  position: relative;
  max-width: 100%;
  overflow: hidden;
}

.indicators {
  position: absolute;
  bottom: 20px;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.indicators span {
  width: 10px;
  height: 10px;
  background-color: #bbb;
  display: inline-block;
  margin: 0 20px;
  border-radius: 50%;
  cursor: pointer;
}

.indicators span.active {
  background-color: #09c2dd;
  transform: scale(1.2);
  transition: transform 0.5s; 
}

.fade-enter, .fade-leave-to {
  opacity: 0;
}

.carousel-image {
  width:100%;
  height: 1050px;
  object-fit: cover;
}


.overlay-menu {
  position: absolute;
  top: 0;
  left: 0 ;
  width: 100%;
  list-style: none;
  padding: 10px;
}
.overlay-menu img {
  max-width: 350px; 
}
.overlay-menu li {
  margin: 10px 0;
  font-size: 18px;
  color: #fff;
  cursor: pointer;
}
.overlay-menu a {
  text-decoration: none;
  color: white;
  text-transform: uppercase;
  font-size: 1.1rem;
  font-family: "Poppins", Sans-serif;

}
.fa-magnifying-glass{
  font-size: 1.7rem;
  color:  #09c2dd;
  margin-bottom: 10px;
}
.fa-magnifying-glass:hover{
  color: black;
  cursor: pointer;
}
.titolo {
  list-style: none;
  padding: 0;
  margin-top: 300px;
  margin-left: 200px;
}
.titolo h1{
  font-family: "Poppins", Sans-serif;
  font-size: 130px;
  font-weight: 700;
  color: white;
}
.titolo p{
  color: white;
  margin-left: 20px;
  font-size: 2rem;
  line-height: 1.4em;
  font-family: "Poppins", Sans-serif;

}
 .btn{
  color: white;
  margin-left: 20px;
  margin-top: 20px;
  font-size: 1.4rem;
  border-radius: 5px;
  border: 1px solid white;
  padding: 10px 30px;
  font-family: "Poppins", Sans-serif;

}
.btn:hover{
  background-color: black;
  color: white;
}
.overlay-menu-2 {
  position: absolute;
  top: 35%;
  left: 0 ;
  width: 100%;
  list-style: none;
  padding: 10px;
}
 h2{
  font-size: 5rem;
  line-height: 1.2em;
  font-family: "Poppins", Sans-serif;
  font-weight: 700;
}
.overlay-menu-2 p {
  font-size: 1.8rem;
  line-height: 1.4em;
  font-family: "Poppins", Sans-serif;
}
.overlay-menu-3 {
  position: absolute;
  top: 35%;
  left: 0 ;
  width: 100%;
  list-style: none;
  padding: 10px;
}
.overlay-menu-3 p {
  font-size: 1.4rem;
  line-height: 1.4em;
  font-family: "Poppins", Sans-serif;
}
a:hover{
  color: #09c2dd;
}
.dropdown {
  position: relative;
  display: inline-block;
  line-height: 1.8em;
}


.dropdown-content {
  display: none;
  position: absolute;
  background-color: #09c2dd;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  z-index: 1000; 
  top: 100%; 
  left: 0%; 
  margin-top: 10px;
  min-width: 200px;


  }

.dropdown-content a {
  color: white;
  padding: 5px 0px;
  padding-right: 70px;
  padding-left: 5px;
  text-decoration: none;
  display: block;
  font-size: 0.8rem;

}
.dropdown-content a:hover {color: black;}

.dropdown:hover .dropdown-content {display: block;}

.dropdown-content li {
  list-style: none;
  margin-left: 0;
  
}
.dropdown-content ul {
  padding-left: 0;
}
</style>
