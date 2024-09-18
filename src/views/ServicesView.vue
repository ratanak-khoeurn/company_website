<template>
  <NavBar />
  <div class="service_page">
    <div class="service_top">
      <h1 data-aos="fade-right">Comprehensive Solutions for Every Need</h1>
      <span data-aos="fade-left"
        >In technology refers to a holistic approach that addresses diverse
        challenges across various sectors. This can include integrated software
        systems, cloud computing services, data analytics, and cybersecurity
        measures. <br /><br />
        By offering tailored solutions, organizations can optimize operations,
        enhance productivity, and ensure robust protection against threats, all
        while adapting to the evolving landscape of technology. Whether for
        businesses, educational institutions, or individual users, these
        solutions aim to streamline processes and foster innovation.</span
      >
    </div>
    <div class="container">
      <div class="ourView">
        <img src="@/assets/service/meeting.svg" alt="meeting" data-aos="fade-right" />
        <h5 data-aos="fade-left">
          We enable our clients to accomplish and enjoy the value of operational
          excellence using our innovative data-driven technological solutions.
        </h5>
      </div>

      <div class="service_card_top">
        <div class="micro_card1" data-aos="fade-right">
          <div class="card_header">
            <h5 class="card_title">University Resources Management System</h5>
            <div class="row_up">
              <img src="../assets/service/link.png" alt="row_up" />
            </div>
          </div>
          <div class="card_des">
            <span class="text">
              Our University Resources Management System (URMS) is designed to
              simplify the complexities of higher education administration. From
              student enrollment to faculty management, URMS provides a
              seamless, integrated platform that enhances operational
              efficiency, improves resource allocation, and fosters academic
              excellence.
            </span>
          </div>
          <br />
          <div class="card_img"></div>
        </div>
        <div class="micro_card2" data-aos="fade-left">
          <div class="card_header">
            <h5 class="card_title">K-12 School Management System</h5>
            <div class="row_up">
              <img src="../assets/service/link.png" alt="row_up" />
            </div>
          </div>
          <div class="card_des">
            <span class="text">
              Our K-12 School Management System is a comprehensive solution that
              caters to the unique needs of primary and secondary education
              institutions. It simplifies administrative tasks, enhances
              communication, and supports teachers in delivering quality
              education, all while keeping parents informed and engaged.
            </span>
          </div>
          <br />
          <div class="card_img"></div>
        </div>
      </div>
      <div class="service_card_mid">
        <div class="micro_card3" data-aos="fade-right">
          <div class="card_header">
            <h5 class="card_title">Medical Clinic Management System</h5>
            <div class="row_up">
              <img src="../assets/service/link.png" alt="row_up" />
            </div>
          </div>
          <div class="card_des">
            <span class="text">
              Healthcare is complex, but managing it shouldn’t be. Our Medical
              Clinic Management System offers a streamlined approach to clinic
              management, ensuring that patient care remains the top priority.
              From scheduling to billing, every feature is designed with
              simplicity and efficiency in mind.
            </span>
          </div>
          <br />
          <div class="card_img"></div>
        </div>
        <div class="micro_card4" data-aos="fade-left">
          <div class="card_header">
            <h5 class="card_title">HR Management System</h5>
            <div class="row_up">
              <img src="../assets/service/link.png" alt="row_up" />
            </div>
          </div>
          <div class="card_des">
            <span class="text">
              Our HR Management System is designed to handle the full spectrum
              of human resource activities with ease. From recruitment and
              onboarding to performance management and payroll, our system helps
              you manage your workforce more effectively, driving employee
              satisfaction and organizational success.
            </span>
          </div>
          <br />
          <div class="card_img"></div>
        </div>
      </div>
      <div class="service_card_bottom">
        <div class="micro_card5" data-aos="fade-right">
          <div class="card_header">
            <h5 class="card_title">CRM (Customer Relationship Management)</h5>
            <div class="row_up">
              <img src="../assets/service/link.png" alt="row_up" />
            </div>
          </div>
          <div class="card_des">
            <span class="text">
              Our CRM system is more than just a tool—it's your strategy for
              building lasting customer relationships. With a focus on
              personalization, engagement, and data-driven insights, our CRM
              helps you understand your customers better, improve customer
              service, and drive sales growth.
            </span>
          </div>
          <br />
          <div class="card_img"></div>
        </div>
        <div class="micro_card6" data-aos="fade-left">
          <div class="card_header">
            <h5 class="card_title">Accounting and Finance Management System</h5>
            <div class="row_up">
              <img src="../assets/service/link.png" alt="row_up" />
            </div>
          </div>
          <div class="card_des">
            <span class="text">
              Our Accounting and Finance Management System takes the complexity
              out of financial management. Designed for accuracy and efficiency,
              our system provides comprehensive tools for managing accounts,
              budgets, invoices, and financial reporting, helping you make
              informed financial decisions with confidence.
            </span>
          </div>
          <br />
          <div class="card_img"></div>
        </div>
      </div>
    </div>
  </div>
  <FooTer></FooTer>
</template>

<script>
// @ is an alias to /src
import NavBar from "@/components/NavBar.vue";
import FooTer from "@/components/FooTer.vue";

export default {
  components: {
    NavBar,
    FooTer,
  },
};
</script>

<style>
.service_page {
  background-color: #f8f7f5;
  margin-top: 50px;
  margin-bottom: -80px;
  width: 100%;
  padding: 50px;
  padding-bottom: 100px;
  display: flex;
  flex-direction: column;
}

.service_top {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  margin: 50px;
  padding: 30px 0px 0 10px;
}
.service_top h1,
.card_title,
.ourView {
  color: #0f58a8;
}
.service_top span {
  width: 85%;
}
.ourView {
  display: flex;
  flex-direction: column;
  margin-top: -20px;
  gap: 2rem;
  width: 100%;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.ourView img {
  width: 100%;
  background-repeat: no-repeat;
}
.ourView h5 {
  width: 75%;
}
.container {
  display: flex;
  flex-direction: column;
  margin-top: 50px;
  width: 100%;
}
.service_card_top,
.service_card_bottom {
  display: flex;
  justify-content: space-between;
  margin-top: 50px;
  height: 600px;
  width: 100%;
}

.micro_card1,
.micro_card2,
.micro_card5,
.micro_card6 {
  display: flex;
  background-color: white;
  border-radius: 20px;
  padding: 20px;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.card_des {
  display: flex;
  width: 100%;
  text-align: left;
  height: 130px;
  overflow-y: scroll;
  gap: 10px;
  overflow-x: hidden;
}
.card_des::-webkit-scrollbar {
  width: 0px;
  height: 0px;
}
.card_des {
  scrollbar-width: none;
}
.card_des {
  -ms-overflow-style: none;
}

.micro_card1,
.micro_card5 {
  display: flex;
  width: 45%;
  height: 600px;
}
.micro_card2,
.micro_card6 {
  display: flex;
  width: 52%;
  height: 600px;
}

.service_card_mid {
  display: flex;
  justify-content: space-between;
  margin-top: 50px;
  width: 100%;
  height: 600px;
}
.micro_card3,
.micro_card4 {
  display: flex;
  background-color: white;
  border-radius: 20px;
  padding: 20px;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.micro_card3 {
  display: flex;
  padding: 20px;
  width: 52%;
  height: 600px;
}
.micro_card4 {
  display: flex;
  width: 45%;
  height: 600px;
}
.card_header {
  display: flex;
  width: 100%;
  justify-content: space-between;
  align-items: center;
}
.micro_card1 .card_img,
.micro_card2 .card_img,
.micro_card5 .card_img,
.micro_card3 .card_img,
.micro_card4 .card_img,
.micro_card6 .card_img {
  width: 100%;
  border-radius: 20px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  height: 350px;
  background-size: cover;
}
.micro_card1 .card_img {
  background-image: url("@/assets/service/product1.svg");
}
.micro_card2 .card_img {
  background-image: url("@/assets/university/school.jpg");
}
.micro_card3 .card_img {
  background-image: url("@/assets/service/product3.svg");
}
.micro_card4 .card_img {
  background-image: url("@/assets/service/product4.svg");
}
.micro_card5 .card_img {
  background-image: url("@/assets/service/product5.svg");
}
.micro_card6 .card_img {
  background-image: url("@/assets/service/product6.svg");
}

/* Mobile Styles (up to 600px) */
@media (max-width: 767px) {
  .service_top {
    display: flex;
    flex-direction: column;
    gap: 2rem;
    margin: 0px 0px 10px 0px;
    padding: 30px 0px 0 10px;
  }
  .service_page {
    padding: 20px;
  }

  .service_top h1,
  .ourView h5 {
    font-size: 1.5rem;
    width: 100%;
  }

  .service_top span {
    width: 100%;
  }

  .ourView img {
    width: 100%;
  }

  .container {
    margin-top: 20px;
  }

  .service_card_top,
  .service_card_mid,
  .service_card_bottom {
    flex-direction: column;
    align-items: center;
    height: auto;
  }

  .micro_card1,
  .micro_card2,
  .micro_card3,
  .micro_card4,
  .micro_card5,
  .micro_card6 {
    width: 100%;
    height: auto;
    margin-bottom: 20px;
  }

  .micro_card1 .card_img,
  .micro_card2 .card_img,
  .micro_card3 .card_img,
  .micro_card4 .card_img,
  .micro_card5 .card_img,
  .micro_card6 .card_img {
    height: 200px;
  }
}

/* Tablet Styles (600px to 900px) */
@media (min-width: 768px) and (max-width: 1024px) {
  .service_top {
    display: flex;
    flex-direction: column;
    width: 100%;
    gap: 2rem;
    margin: 0px 0px 10px 0px;
    padding: 30px 0px 0 10px;
  }
  .service_page {
    padding: 30px;
  }

  .service_top h1 {
    font-size: 2rem;
  }
  .service_top span {
    width: 100%;
  }
  .ourView h5 {
    font-size: 1.2rem;
  }
  .card_title {
    display: flex;
    align-items: center;
    overflow-y: auto;
    width: 100%;
    height: 40px;
  }
  .service_card_top,
  .service_card_mid,
  .service_card_bottom {
    align-items: center;
    height: 500px;
  }

  .micro_card1,
  .micro_card2,
  .micro_card3,
  .micro_card4,
  .micro_card5,
  .micro_card6 {
    width: 48%;
    height: 100%;
    margin-bottom: 30px;
  }

  .micro_card1 .card_img,
  .micro_card2 .card_img,
  .micro_card3 .card_img,
  .micro_card4 .card_img,
  .micro_card5 .card_img,
  .micro_card6 .card_img {
    height: 250px;
  }
}
</style>
