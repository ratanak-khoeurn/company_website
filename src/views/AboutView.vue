<template>
  <div class="home" style="background-color: #f8f7f5">
    <NavBar />
    <div class="container">
      <div class="banner">
        <img src="@/assets/image/about_us.svg" alt="banner" />
      </div>
      <div class="history">
        <h1 data-aos="fade-right">Vectorasoft History</h1>
        <p class="bank_history" data-aos="fade-left">
          Vectorasoft is a leading provider of business and education software
          solutions, dedicated to transforming the way organizations operate.
          With a team of experts in software development, data science, and
          business intelligence. We create innovative products that empower our
          clients to achieve their goals. Our commitment to excellence, customer
          success, and technological innovation sets us apart as a trusted
          partner in your journey to success.
        </p>
      </div>
      <div class="grid-container bank_image">
        <div class="grid-container-left">
          <div class="grid-item image_1" data-aos="fade-right">
            <img src="@/assets/university/students.jpg" alt="History 1" />
          </div>
          <div class="grid-item image_2" data-aos="fade-right">
            <img src="@/assets/university/contact_form.png" alt="History 2" />
          </div>
        </div>
        <div class="history_right">
          <div class="grid-item image_3" data-aos="fade-left">
            <img src="@/assets/university/product.jpg" alt="History 3" />
          </div>
          <div class="grid-item-right_bottom">
            <div class="grid-item black-box">
              <h6>Explore Our Solutions</h6>
              <h4>Why Choose <span> Vectorasoft?</span></h4>
            </div>
            <div class="grid-item image_4" data-aos="fade-right">
              <img src="@/assets/university/dashboard.jpg" alt="History 4" />
            </div>
          </div>
        </div>
      </div>
      <br />
      <br />
      <div class="description">
        <span data-aos="fade-right"
          >At Vectorasoft, we believe that technology should be simple,
          powerful, and transformative. Our mission is to craft software
          solutions that empower businesses to achieve more with less. We focus
          on practical innovation—delivering tools that solve real problems,
          enhance productivity, and drive growth. Our expertise spans across
          industries, from education and healthcare to finance and business
          management. Let’s collaborate to transform your operations and achieve
          our shared goals. Together, we can leverage our powerful,
          user-friendly software solutions to drive mutual growth and contribute
          to a better society
        </span>
        <br />
        <br />
        <h4 data-aos="fade-left">Security and Quality</h4>
        <span data-aos="fade-right">
          With our team’s experiences working with banks and educational
          institutions, we truly care for both quality and security in the
          products we made. Our dedicated quality assurance team constantly
          overseas issues and suggest solutions.
        </span>
        <br />
        <br />
        <h4 data-aos="fade-left">Creative and Capability</h4>
        <span data-aos="fade-left">
          We have highly skilled engineers with excellent technical knowledge
          and experience in using latest software standards, tools, platforms,
          frameworks and technologies and we invest continuously in training and
          education, to be able to respond to any new technology challenges and
          requirements from our clients.
        </span>
        <br />
        <br />
        <h4 data-aos="fade-left">Team's Technical Strengths</h4>
        <span>
          1. Deep and extensive experiences within university context
          <br />
          2. We only need minimal instruction or guidelines to deliver a working
          solution.
          <br />
          3. Real experiences in leading and development of University Resources
          Management System (URMS) since 2015.
          <br />
          4. Highly creative in developing algorithm with deep understanding of
          business requirements.
          <br />
          5. Strong technical experiences and know-how for both proprietary (C#,
          MSSQL, Web Services) and open-source (such as PHP, Laravel, MySql)
          development environments.
          <br />
          6. We have capability of combining various technologies to suit
          customers’ needs.
          <br />
          7. Ability to make complicated things as simple as possible.
        </span>
      </div>
      <div class="mis_vis">
        <div class="vission">
          <div class="grid-item-vission">
            <img src="../assets/image/rank.png" alt="Vission" data-aos="fade-right"/>
            <div class="vis_info" data-aos="fade-left">
              <h1>Our Vission</h1>
              <p>
                At Vectorasoft, we aspire to be at the forefront of a global
                transformation by cultivating deep partnerships that harness the
                evolving power of technology and the growth of intelligence. We
                believe in the convergence of diverse disciplines to create
                solutions that align with the fundamental truths of nature. By
                nurturing and digitizing intelligence, we aim to craft a future
                where knowledge and technology work in harmony, driving
                meaningful advancements for industries and enriching lives.
              </p>
            </div>
          </div>
          <div class="grid-item-mission">
            <div class="mission_info" data-aos="fade-right">
              <h1>Our Mission</h1>
              <p>
                Our mission at Vectorasoft is to build transformative
                partnerships that harness the power of technology and innovative
                learning. We create solutions designed to help businesses and
                institutions achieve more with less—boosting productivity and
                efficiency through the intelligent use of resources. By
                integrating diverse expertise and leveraging cutting-edge
                technology, we drive impactful results that enable our partners
                to excel and thrive in a rapidly evolving world.
              </p>
            </div>
            <img src="../assets/image/working3.png" alt="mission" data-aos="fade-left"/>
          </div>
        </div>
      </div>
      <div class="quote" data-aos="fade-left">
        <p>
          "To build transformative partnerships that harness technology and
          innovative learning, empowering businesses and institutions to boost
          productivity and achieve more with less."
        </p>
      </div>
    </div>
    <Footer></Footer>
  </div>
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import Footer from "@/components/FooTer.vue";
export default {
  name: "AboutView",
  components: {
    NavBar,
    Footer,
  },
};
</script>

<style scoped>
.about {
  background-color: #f8f7f5;
  padding-top: 50px;
}
.banner {
  background-size: cover;
  width: 100%;
  height: 500px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
.banner img {
  width: 100%;
  object-fit: cover;
}
.history {
  padding: 5rem 0;
  margin-top: -100px;
  width: 100%;
  align-items: center;
  justify-content: center;
  text-align: center;
}
.bank_history {
  display: flex;
  width: 100%;
  padding: 50px 200px 0px 200px;
}
.description,
.history,
.grid-item-mission,
.grid-item-vission {
  color: #5b6068;
}
.grid-item-vission img,
.grid-item-mission img {
  border-radius: 30px;
  height: 70vh;
}
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;
}

.grid-container-left {
  display: grid;
  grid-template-columns: repeat(1fr);
  grid-template-rows: 2fr;
  gap: 1rem;
}

.history_right {
  display: grid;
  grid-template-columns: repeat(1, 1fr);
  grid-template-rows: 2fr;
  gap: 1rem;
}

.grid-item {
  position: relative;
}

.grid-item img {
  width: 100%;
  border-radius: 10px;
}

.black-box {
  background-color: #0f58a8;
  color: white;
  padding: 2rem;
  display: flex;
  margin-bottom: 50%;
  width: 300px;
  height: 300px;
  flex-direction: column;
  justify-content: center;
  border-radius: 10px;
  box-shadow: inset 0px -100px 100px #0a151b; /* Inner shadow at the bottom */
}
.black-box h6 {
  font-style: italic;
}
.black-box h4 {
  margin-top: 10px;
  font-weight: bold;
}
.black-box h4 span {
  display: flex;
  margin-top: 10px;
  margin-left: 40px;
}
.grid-item-vission,
.grid-item-mission {
  display: grid;
  margin-top: 50px;
  grid-template-columns: repeat(2, 1fr);
  gap: 1rem;
}
.quote {
  font-weight: bold;
  font-size: 20px;
  padding: 5% 10% 0% 10%;
  text-align: center;
}
.grid-item-right_bottom {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1rem;
}

.image_1 > img {
  width: 400px;
  height: 490px;
  margin-left: 20%;
}

.image_2 > img {
  width: 500px;
  height: 63vh;
}

.image_3 > img {
  margin-top: 100px;
  width: 90%;
  height: 55vh;
}

.image_4 > img {
  width: 450px;
  height: 55vh;
}
.history h1,
.grid-item-mission h1,
.grid-item-vission h1,
.quote,
.description span h4 {
  color: #0f58a8;
}
.grid-item-mission img:hover,
.grid-item-vission img:hover,
.social > a > img:hover,
.image_1 > img:hover,
.image_2 > img:hover,
.image_3 > img:hover,
.image_4 > img:hover {
  filter: brightness(1.2);
  transition: filter 0.1s ease-in-out;
  transition: transform 0.3s ease-in-out;
  transform: scale(1.03);
  cursor: pointer;
}

@media (min-width: 768px) and (max-width: 1024px) {
  .banner {
    display: flex;
    width: 100%;
    background-size: cover;
    height: 300px;
    align-items: center;
    flex-direction: column;
  }
  .banner img {
    width: 100%;
    object-fit: cover;
  }
  .history {
    font-size: 14px;
  }
  .bank_history {
    padding: 10px;
  }
  .grid-container {
    grid-template-columns: 1fr;
  }
  .black-box {
    width: 100%;
    margin: 10px auto;
  }
  .quote {
    font-size: 16px;
  }
  .image_1 > img {
    width: 345px;
    height: 300px;
    margin-left: 0px;
  }

  .image_2 > img {
    width: 340px;
    height: 300px;
  }

  .image_3 > img {
    margin-top: 0px;
    width: 100%;
    height: 300px;
  }

  .image_4 > img {
    width: 430px;
    height: 250px;
  }
  .grid-container-left {
    display: flex;
  }
  .history_right {
    display: flex;
    flex-direction: column;
    width: 100%;
    top: 0;
  }
  .black-box {
    margin-top: 0;
    width: 250px;
    height: 250px;
  }
  .grid-item-vission,
  .grid-item-mission {
    display: flex;
    width: 100%;
  }
  .grid-item-vission img,
  .grid-item-mission img {
    width: 100%;
    height: 300px;
  }
}
@media (min-width: 428px) and (max-width: 767px) {
  .banner {
    display: flex;
    width: 100%;
    background-size: cover;
    height: 300px;
    align-items: center;
    flex-direction: column;
  }
  .banner img {
    width: 100%;
    object-fit: cover;
  }
  .history {
    font-size: 14px;
  }
  .bank_history {
    padding: 10px;
  }
  .grid-container {
    grid-template-columns: 1fr;
  }
  .black-box {
    width: 100%;
    margin: 10px auto;
  }
  .quote {
    font-size: 16px;
  }
  .image_1 > img {
    width: 100%;
    height: 220px;
    margin-left: 0px;
  }

  .image_2 > img {
    width: 100%;
    height: 220px;
  }

  .image_3 > img {
    margin-top: 0px;
    width: 100%;
    height: 220px;
  }

  .image_4 > img {
    width: 100%;
    height: 200px;
  }
  .grid-container-left {
    display: flex;
    width: 100%;
    flex-direction: column;
  }
  .history_right {
    display: flex;
    flex-direction: column;
    width: 100%;
    top: 0;
  }
  .black-box {
    margin-top: 0;
    width: 250px;
    height: 200px;
  }
  .grid-item-vission,
  .grid-item-mission {
    display: flex;
    flex-direction: column;
    width: 100%;
  }
  .grid-item-vission img,
  .grid-item-mission img {
    width: 100%;
    height: 300px;
  }
}
</style>
