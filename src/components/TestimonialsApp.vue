<template>
    <section>
      <div class="container">
        <h2 class="text-center">Testimonials</h2>
        <div class="line">
          <div class="black"></div>
          <div class="blue"></div>
          <div class="black"></div>
        </div>
  
        <div class="row">
          <div class="col-10 py-5 d-flex align-items-center">
            <img
              :src="testimonials[currentIndex].image"
              alt="logo-person"
              @mousedown="startAutoPlay"
              @mouseup="stopAutoPlay"
              @mouseleave="stopAutoPlay"
              class="carousel-image"
            />
            <div class="content">
              <p class="font">{{ testimonials[currentIndex].text }}</p>
              <h6 class="text-white">{{ testimonials[currentIndex].author }}</h6>
            </div>
          </div>
        </div>
        <div class="indicators">
          <span
            v-for="(testimonial, index) in testimonials"
            :key="index"
            @click.prevent.native="goToImage(index)"
            :class="{ active: index === currentIndex }"
          ></span>
        </div>
      </div>
    </section>
  </template>
  
  
  <script>
  import '@fortawesome/fontawesome-free/css/all.css';
  
  export default {
    name: 'TestimonialsApp',
    data() {
      return {
        currentIndex: 0,
        testimonials: [
          {
            image: "/src/assets/images/person0-p0a17bbqv6696rzdb2ly3jl0kdng6od3fj7vti5wi8.jpg",
            text:   "As a yacht owner, after either of my regular maintenance checkups, I oftentimes find it necessary to do this or that kind of a repair. The thing is that I don’t always have enough time (or sometimes the skill) to do all of the repairs all by myself…",
            author: "-Albert Winning",
          },
          {
            image: "/src/assets/images/person01-p0a17bbqv6696rzdb2ly3jl0kdng6od3fj7vti5wi8.jpg",
            text:  "Having had a real handful of favorite pastimes over the course of my whole adult life, sailing was always front and center in such a list. So, when I found out about this yachts chartering service located just a few miles near my home, I was thrilled!",
            author: "-Reginald Stanhow",
          },
          {
            image: "/src/assets/images/person03-p0a17bbqv6696rzdb2ly3jl0kdng6od3fj7vti5wi8.jpg",
            text: "I am an event manager who works for one of the Fortune 500 US-based companies. From time to time, we throw some awesome corporate, large-scale corporate events, as a gesture of appreciation to our employees. Yacht chartering is one of those!",
            author: "-Mary Adwetto",
          },
        ],     
       };
    },
    methods: {
      goToImage(index) {
        this.currentIndex = index;
      },
      startAutoPlay() {
        this.changeImage(1);
      },
      stopAutoPlay() {
        // Leave it empty, as we don't want to change images when the click is released
      },
      changeImage(offset) {
        const newIndex = this.currentIndex + offset;
        if (newIndex >= 0 && newIndex < this.testimonials.length) {
          this.currentIndex = newIndex;
        }
      },
}
}
  </script>
  
  <style lang="css" scoped>
  .scroll-to-top {
  position: fixed;
  bottom: 20px;
  right: 20px;
  cursor: pointer;
  border-radius: 50%;
}

.scroll-to-top i {
  color: black;
  font-size: 20px;
}
  section {
    margin: 0;
    background-image: url(../assets/images/bg8.jpg);
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    overflow: hidden;
    min-height: 700px;
  }
  .line {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 30px 0;
  }
  .blue {
    width: 5%;
    height: 2px;
    background-color: white;
  }
  .black {
    width: 55%;
    height: 1px;
    background-color: lightgrey;
  }
  h2 {
    font-size: 2.5em;
    color: white;
    font-weight: 700;
    padding-top: 100px;
    padding-bottom: 20px;
  }
  .col-10 {
    background-color: rgba(169, 169, 169, 0.5);
  }
  img {
    border-radius: 50%;
    margin-left: 20px;
    max-width: 100%;
  }
  .content {
    max-width: 70%;
    color: rgba(255, 255, 255, 0.7);
  }
  .content p {
    font-size: 1.2em;
    line-height: 1.5em;
  }
  .font {
    position: relative;
  }
  .font::before {
    content: "\f10e";
    font-family: 'Font Awesome 5 Free';
    font-weight: 900;
    font-size: 4em;
    color: rgba(255, 255, 255, 0.5);
    position: absolute;
    top: -15px;
    left: 0;
  }
  .indicators {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 100px;
}

.indicators span {
  width: 15px;
  height: 15px;
  background-color:transparent;
  border: 2px solid white;
  display: inline-block;
  margin: 0 20px; 
  border-radius: 50%;
  cursor: pointer;
}

.indicators span.active {
  background-color:white;
  transform: scale(1.3);
  transition: transform 0.5s;
}
  </style>
  