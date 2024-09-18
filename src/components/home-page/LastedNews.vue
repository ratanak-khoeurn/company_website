<template>
  <div class="title-last-news">
    <h1 data-aos="fade-right">Latest News of Company</h1>
    <a href=""
      data-aos="fade-left"><img src="@/assets/home/icon_enter.svg" alt="" />View All Blog</a
    >
  </div>
  <div class="card-news">
    <div class="card_top">
      <div class="news-card1" data-aos="fade-right">
        <div class="card-1">
          <div class="news-card-content">
            <h2 class="news-card-title">Our Team</h2>
            <hr />
            <p class="news-card-text">
              Welcome to Vectorasoft, a leading provider of intelligent data
              driven solutions, specializing in business application development
              and consultancy in operational optimization using our
              state-of-the-arts engineering capability, and experiences. Our
              tech solutions can be delivered as enterprise-level licenses or
              subscription services, tailor-made or industrial standard. With
              our unique engineering know-how, we are proud to provide
              cost-effective top-notch solutions, which can create greater
              values in your businesses and deliver higher level of customer
              satisfaction.
            </p>
            <div class="img_bg">
              <img src="@/assets/university/vectora.jpg" alt="News Image" />
            </div>
            <p class="news-card-date">January 20, 2024</p>
          </div>
        </div>
      </div>
      <div class="news-card2" data-aos="fade-left">
        <div class="card-1">
          <div class="news-card-content">
            <h2 class="news-card-title">Our Achivement</h2>
            <hr />
            <p class="news-card-text">
              is a software solution designed to manage the lifecycle of loans
              from origination to repayment. It automates processes such as
              application processing, credit assessment, disbursement, and
              collections.
            </p>
            <div class="img_bg">
              <img src="@/assets/university/dashboard.jpg" alt="News Image" />
            </div>
            <p class="news-card-date">Aprile 20, 2024</p>
          </div>
        </div>
      </div>
    </div>
    <div class="card_bottom">
      <div class="news-card3" data-aos="fade-right">
        <div class="card-1">
          <div class="news-card-content">
            <h2 class="news-card-title">Our Planing</h2>
            <hr />
            <p class="news-card-text">
              1. Project Idea Define the Objective: What is the core purpose of
              the project? Why is it needed? Target Audience: Who is this
              project for? Identify your audience and how they will benefit from
              the project. Desired Outcome: What do you want to achieve by
              creating this? List the key features or results. <br />2. Research
              & Inspiration Competitor Analysis: Check out existing solutions
              similar to what you want to build. Understand their strengths and
              weaknesses. Inspiration: Gather ideas from multiple sources, like
              successful projects, UI/UX design inspirations, or relevant
              technologies. Technology Stack: Select the technologies,
              languages, and frameworks you'll use to build this (e.g., Laravel,
              Vue.js, React, Node.js). <br />
              3. Brainstorm Features Core Features: List the must-have features
              of your project. These are the essential components without which
              your project will fail. Secondary Features: What additional
              features would add value? These may not be necessary but could
              differentiate your project. User Stories: Think about how users
              will interact with the product. Write simple “user stories” that
              describe these interactions. <br />4. Design Phase Wireframes:
              Create rough sketches or wireframes to map out what each screen or
              feature will look like. Tools like Figma, Sketch, or Adobe XD can
              help. Prototyping: Build a prototype if necessary, especially for
              interactive elements. This will help you visualize the user
              journey. UI/UX Design: Focus on user experience and user
              interface, ensuring that the design is intuitive and visually
              appealing. <br />5. Project Structure Set Up Repository:
              Initialize a GitHub or GitLab repository for version control.
              Break the Project into Phases: Divide the development into
              multiple phases, such as MVP (Minimum Viable Product), Alpha,
              Beta, and Final Release. Roadmap: Create a project roadmap with
              milestones and deadlines. <br />6. Development Phase 1: MVP
              (Minimum Viable Product): Backend Development: Set up your
              database and server-side functionality. Define API endpoints and
              ensure data models are in place. Frontend Development: Create the
              UI/UX and connect it to the backend. Ensure key pages are
              functional, e.g., user registration/login, dashboard, etc. Phase
              2: Core Features Implementation: Implement the core features based
              on the user stories. Focus on completing high-priority features
              first. Phase 3: Secondary Features: Add secondary features and
              improvements. Start with those that enhance the user experience.
              <br />7. Testing Unit Testing: Ensure each module works as
              expected by writing unit tests. Integration Testing: Ensure that
              components work together correctly. User Testing: Allow a small
              group of users to interact with the product and gather feedback on
              the user experience. Bug Fixes: After testing, address any issues
              or bugs encountered.
            </p>
            <div class="img_bg">
              <img src="@/assets/university/plan.jpg" alt="News Image" />
            </div>
            <p class="news-card-date">May 20, 2024</p>
          </div>
        </div>
      </div>
      <div class="news-card4" data-aos="fade-left">
        <div class="card1">
          <div class="news-card-content">
            <h2 class="news-card-title">Our Products</h2>
            <hr />
            <p class="news-card-text">
              With increasing digitization, come the risk of data and digital
              trust. Our system solutions have passed rigorous tests by the
              security team at our bank partners. Our dynamic Research &
              Development team is also progressively exploring and updating the
              security measures in our coding as well as infrastructure
              configuration.
            </p>
            <div class="img_bg">
              <img src="@/assets/university/company.jpg" alt="News Image" />
            </div>
            <p class="news-card-date">December 20, 2024</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "LastedNews",
};
</script>

<style>
.title-last-news {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
  max-width: 100%;
  margin-top: 30px;
  margin: 60px;
}
.title-last-news a {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 1rem;
}
.title-last-news a img{
  width: 40px;
  height: 40px;
}
.card-news {
  display: flex;
  flex-direction: column;
  width: 100%;
  justify-content: center;
}
.card_top,
.card_bottom {
  display: flex;
  width: 90%;
  height: auto;
  margin-left: 70px;
  gap: 3rem;
  align-items: center;
}
.card_bottom {
  display: flex;
  margin-top: 50px;
}
.news-card3,
.news-card2 {
  display: flex;
  width: 700px;
  background-color: #fff;
  box-shadow: 0 2px 6px rgba(36, 34, 34, 0.1);
  border-radius: 32px;
  overflow: hidden;
}
.news-card1,
.news-card4 {
  background-color: #fff;
  box-shadow: 0 2px 6px rgba(0, 0, 0, 0.1);
  border-radius: 32px;
  overflow: hidden;
  width: 600px;
}

.img_bg {
  width: 100%;
  height: 420px;
  background-position: center;
  background-repeat: no-repeat;
  border-radius: 30px;
  margin-top: 20px;
  transition: background-color 0.3s ease;
  background-size: cover;
}

.img_bg img {
  width: 100%;
  height: 100%;
  border-radius: 20px;
  background-position: center;
}

.news-card-content {
  padding: 20px;
}

.news-card-title {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 10px;
}

.news-card-text {
  width: 100%;
  height: 100px;
  overflow-y: auto;
  overflow-x: hidden;
  font-size: 16px;
  line-height: 1.5;
  margin-bottom: 20px;
  scrollbar-width: none;
  -ms-overflow-style: none;
}
.news-card-text::-webkit-scrollbar {
  width: 0px;
  height: 0px;
}
.news-card-date {
  font-size: 14px;
  text-align: right;
  margin-top: 10px;
}

/* Responsive styles */
@media (min-width: 428px) and (max-width: 767px) {
  .news-card {
    display: flex;
    flex-direction: column;
    max-width: 100%;
  }
  .card_top,
  .card_bottom {
    display: flex;
    flex-direction: column;
    width: 100%;
    margin-left: 15px;
  }
  .title-last-news {
    display: flex;
    flex-direction: column;
    align-items: start;
    padding-left: 0;
    width: 100%;
    margin-left: 20px;
    margin-top: 20px;
  }
  .title-last-news h1 {
    display: flex;
    font-weight: bold;
    font-size: 20px;
    margin-bottom: 10px;
  }
  .title-last-news a img {
    width: 30px;
    height: 30px;
    margin-right: 10px;
  }
  .img_bg {
    height: 250px;
  }

  .news-card-title {
    font-size: 20px;
  }

  .news-card-text {
    font-size: 14px;
  }

  .news-card-date {
    margin-top: 60px;
    font-size: 12px;
  }
  .news-card3,
  .news-card2,
  .news-card1,
  .news-card4 {
    display: flex;
    width: 100%;
    height: 550px;
    background-color: #fff;
    box-shadow: 0 2px 6px rgba(36, 34, 34, 0.1);
    border-radius: 32px;
    overflow: hidden;
    margin-left: -30px;
    margin-top: -30px;
  }
  .news-card1 img,
  .news-card2 img,
  .news-card3 img,
  .news-card4 img {
    width: 100%;
    height: 300px;
    border-radius: 20px;
  }
}
@media (min-width: 768px) and (max-width: 1024px) {
  .news-card {
    display: flex;
    flex-direction: column;
    max-width: 100%;
  }
  .card_top,
  .card_bottom {
    display: flex;
    flex-direction: column;
    width: 100%;
    margin-left: 15px;
  }
  .title-last-news {
    display: flex;
    width: 100%;
    margin-top: 20px;
    margin-left: 0;
  }
  .title-last-news h1 {
    display: flex;
    font-weight: bold;
    font-size: 20px;
    margin-bottom: 10px;
  }
  .title-last-news a img {
    width: 30px;
    height: 30px;
    margin-right: 10px;
  }
  .img_bg {
    height: 250px;
  }

  .news-card-title {
    font-size: 20px;
  }

  .news-card-text {
    font-size: 14px;
  }

  .news-card-date {
    margin-top: 25%;
    font-size: 12px;
  }
  .news-card3,
  .news-card2,
  .news-card1,
  .news-card4 {
    display: flex;
    width: 95%;
    height: 650px;
    background-color: #fff;
    box-shadow: 0 2px 6px rgba(36, 34, 34, 0.1);
    border-radius: 32px;
    overflow: hidden;
    margin-left: -30px;
  }
  .news-card1 img,
  .news-card2 img,
  .news-card3 img,
  .news-card4 img {
    width: 100%;
    height: 400px;
    border-radius: 20px;
  }
}
</style>
