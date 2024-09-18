<template>
  <div class="News">
    <NavBar />
    <div class="header">
      <h1 class="head_title">
        Meet the bank <br />
        of the future
      </h1>
      <p class="head_info">
        Welcome to the future of banking, where technology and innovation
        redefine the way we work and live. We're here to help you navigate this
        exciting new world. Welcome to the future of banking, where technology
        and innovation redefine the way we work and live. We're here to help you
        navigate this exciting new world.
      </p>
      <button class="btn_start">Get started</button>
    </div>
    <div class="container">
      <div class="middle">
        <div class="mid_top">
          <h2 class="mid_title">News</h2>
          <p class="mid_info">
            A dynamic startup agency, is dedicated to fueling the aspirations of
            emerging businesses. We specialize in crafting captivating online
            identities. A dynamic startup agency, is dedicated to fueling the
            aspirations of emerging businesses. We specialize in crafting
            captivating online identities.
          </p>
        </div>
        <div class="mid_middle">
          <div class="slider">
            <div
              v-for="(slide, index) in slides"
              :key="index"
              :class="[
                'slide',
                `slide${index + 1}`,
                { active: currentSlide === index },
              ]"
              @click="setActiveSlide(index)"
            >
              <div class="detail">
                <img src="@/assets/image/row_up.png" alt="row_up" />
              </div>
              <div class="slide_info">
                <h3>{{ slide.title }}</h3>
                <p>{{ slide.description }}</p>
              </div>
            </div>
          </div>
        </div>
        <div class="mid_bottom">
          <img
            src="@/assets/image/row_left.png"
            alt="row left"
            @click="prevSlide"
          />
          <img
            src="@/assets/image/row_right.png"
            alt="row right"
            @click="nextSlide"
          />
        </div>
      </div>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import Footer from "@/components/FooTer.vue";

export default {
  components: {
    NavBar,
    Footer,
  },
  data() {
    return {
      currentSlide: 0,
      slides: [
        {
          title: "For small business",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        },
        {
          title: "For small business",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        },
        {
          title: "For small business",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        },
        {
          title: "For small business",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
        },
      ],
    };
  },
  methods: {
    setActiveSlide(index) {
      this.currentSlide = index;
    },
    prevSlide() {
      this.currentSlide =
        this.currentSlide > 0 ? this.currentSlide - 1 : this.slides.length - 1;
    },
    nextSlide() {
      this.currentSlide =
        this.currentSlide < this.slides.length - 1 ? this.currentSlide + 1 : 0;
    },
  },
};
</script>

<style scoped>
.News {
  display: flex;
  flex-direction: column;
  background-color: #f8f7f5;
}

.container {
  display: flex;
  flex-direction: column;
  padding: 1px;
  margin: 0;
}

.header {
  background-image: url("@/assets/news/head_bg.png");
  width: 100%;
  height: 640px;
  margin-top: 70px;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  flex-direction: column;
  padding: 10% 8%;
  color: white;
  box-shadow: inset 0 0 205px rgba(0, 0, 0, 0.899); /* shadow inside */
  
}

.head_title {
  font-size: 50px;
}

.head_info {
  font-size: 20px;
  margin-top: 20px;
  line-height: 1.5;
  justify-content: center;
  align-items: center;
  display: flex;
  max-width: 490px;
  height: 200px;
  padding-top: 25px;
  overflow-y: auto;
  scrollbar-width: none;
  -ms-overflow-style: none;
  overflow-x: hidden;
}

.btn_start {
  background-color: #3a358f;
  color: white;
  padding: 10px;
  border: none;
  cursor: pointer;
  border-radius: 50px;
  max-width: 150px;
  margin-top: 20px;
  transition: background-color 0.3s ease;
}

.btn_start:hover {
  filter: brightness(1.7);
  transition: filter 0.3s ease-in-out;
  transition: transform 0.3s ease-in-out;
  transform: scale(1.05);
  cursor: pointer;
}

.middle {
  display: flex;
  flex-direction: column;
  padding: 50px;
}

.mid_top {
  display: flex;
  flex-direction: column;
}

.mid_info {
  font-size: 20px;
  margin-top: 20px;
  line-height: 1.5;
  justify-content: center;
  align-items: center;
  display: flex;
  max-width: 80%;
}

.mid_middle {
  display: flex;
  flex-direction: column;
  margin-top: 50px;
}

.slider {
  margin: 5%;
  display: flex;
  width: 100%;
  height: auto;
  padding: 30px;
  border-radius: 40px;
  gap: 2rem;
  overflow-x: scroll;
  scroll-snap-type: x mandatory;
}

.slider::-webkit-scrollbar {
  display: none;
}

.slide {
  flex: 0 0 auto;
  height: 500px;
  width: 500px;
  gap: 4rem;
  border-radius: 30px;
  margin: 10px;
  display: flex;
  flex-direction: column;
  background-size: cover;
  background-position: center;
  transition: transform 0.5s ease, filter 0.5s ease;
  cursor: pointer;
  box-shadow: inset 0 -200px 50px -20px rgba(0, 0, 0, 0.651); /* shadow inside */
}
.slide1 {
  background-image: url("@/assets/image/team.png");
  height: 500px;
  width: 50%;
  border-radius: 30px;
  background-size: cover;
  background-position: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  transition: background-color 0.3s ease;
  color: white;
}

.slide2 {
  background-image: url("@/assets/image/working1.png");
  height: 500px;
  width: 50%;
  border-radius: 30px;
  background-size: cover;
  background-position: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  transition: background-color 0.3s ease;
  color: white;
}
.slide3 {
  background-image: url("@/assets/image/working2.png");
  height: 500px;
  width: 50%;
  border-radius: 30px;
  background-size: cover;
  background-position: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  transition: background-color 0.3s ease;
  color: white;
}
.slide4 {
  background-image: url("@/assets/image/working3.png");
  height: 500px;
  width: 50%;
  border-radius: 30px;
  background-size: cover;
  background-position: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  transition: background-color 0.3s ease;
  color: white;
}
.slide1:hover,
.slide2:hover,
.slide3:hover,
.slide4:hover {
  filter: brightness(1.07);
  transition: filter 0.3s ease-in-out;
  transition: transform 0.3s ease-in-out;
  transform: scale(1.05);
  cursor: pointer;
}
.detail {
  width: 40px;
  height: 40px;
  border-radius: 100%;
  margin-top: 10px;
  margin-right: 10px;
  align-self: end;
  justify-self: start;
  top: 3px;
  right: 0;
  display: flex;
  background-color: rgba(114, 111, 111, 0.581);
  justify-content: center;
}

.detail > img {
  width: 15px;
  height: 15px;
  margin-top: 12px;
  right: 0;

  display: flex;
}

.detail > img:hover {
  transform: scale(1.1);
  filter: brightness(1.3);
  color: white;
}

.slide_info {
  height: 150px;
  padding-top: 15px;
  overflow-y: auto;
  scrollbar-width: none;
  -ms-overflow-style: none;
  overflow-x: hidden;
  justify-content: center;
  display: flex;
  flex-direction: column;
  gap: 10px;
  margin-top: auto;
  border-radius: 0 0 30px 30px;
  padding: 10px;
  transition: background-color 0.3s ease;
}

.active {
  transform: scale(1.1);
  filter: blur(0);
}

.slide:not(.active) {
  filter: blur(5px);
  opacity: 0.3;
}

/* mid_bottom */
.mid_bottom {
  display: flex;
  text-align: center;
  align-items: center;
  justify-content: center;
  margin-left: 20%;
  cursor: pointer;
  gap: 4rem;
  margin-top: 5%;
  
}

.mid_bottom img {
  width: 40px;
  height: 40px;
}

.mid_bottom img:hover {
  transform: scale(1.2);
  transition: transform 0.3s ease;
}

@media (max-width: 768px) {
  .container {
    padding: 0;
    margin: 0;
  }
  .header {
    width: 100%;
    height: auto;
    margin-top: 30px;
    padding: 20px;
    background-size: contain;
    background-position: center;
  }
  .head_info {
    font-size: 16px;
    line-height: 1.5;
    max-width: 300px;
    height: 100px;
    padding: 10px;
    overflow-y: auto;
    scrollbar-width: none;
    -ms-overflow-style: none;
    overflow-x: hidden;
  }
  .slide {
    width: 200px;
    height: 200px;
  }
  .active {
    width: 300px;
    height: 300px;
  }
}
</style>
