<template>
  <NavBar />
  <div class="contact-us-page">
    <div class="contact">
      <div class="py-3">
        <div class="contact-us-section">
          <h1 class="title" data-aos="fade-right">Have a Question?</h1>
          <p class="sub-title" data-aos="fade-left">
            A dynamic startup agency, is dedicated to fueling the aspirations of
            emerging businesses. We specialize in crafting captivating online
            identities
          </p>
        </div>

        <div class="form-contact">
          <form class="row">
            <h1>Contact Us!</h1>
            <div class="full_name">
              <div class="first_name">
                <label for="first name" class="form-label" data-aos="fade-right">First Name</label>
                <input
                  type="text"
                  placeholder="Enter first name"
                  class="form-control"
                  data-aos="fade-left"
                />
              </div>
              <div class="last_name">
                <label for="last name" class="form-label" data-aos="fade-right">Last Name</label>
                <input
                  type="text"
                  placeholder="Enter last name"
                  class="form-control"
                  data-aos="fade-left"
                />
              </div>
            </div>
            <div class="mail_address">
              <div class="address">
                <label for="email" class="form-label" data-aos="fade-right">Email Address</label>
                <input
                  type="email"
                  class="form-control"
                  placeholder="Enter email Address"
                  id="inputEmail4"
                  data-aos="fade-left"
                />
              </div>
              <div class="phone_number">
                <label for="phone number" class="form-label" data-aos="fade-right"
                  >Phone number</label
                >
                <input
                  type="string"
                  class="form-control"
                  placeholder="Enter phone number"
                  data-aos="fade-left"
                />
              </div>
            </div>
            <div class="col-12">
              <label for="message" class="form-label" data-aos="fade-right">Your Message</label>
              <textarea
                class="form-control"
                rows="3"
                placeholder="Enter your message"
                data-aos="fade-left"
              ></textarea>
            </div>
            <div class="submit">
              <button class="btn_submit" type="submit" data-aos="fade-left">Submit</button>
            </div>
          </form>
        </div>
        <div class="hard-office">
          <div class="office-info">
            <h1 data-aos="fade-right">Book Consultation Appointment</h1>
            <p data-aos="fade-left">
              By integrating technology, organizations can enhance customer
              experience, improve efficiency, and facilitate better
              communication. This approach not only saves time but also allows
              for a more flexible and accessible way to connect with experts,
              whether for technical support, strategic advice, or product
              demonstrations.
            </p>
            <hr />
            <div class="office-contact">
              <div class="contact_left">
                <div class="email_img">
                  <img src="../assets/contact/email.svg" alt="" />
                </div>
                <div class="contact-with-us">
                  <h6 data-aos="fade-right">Mail Us</h6>
                  <p data-aos="fade-left">Vectorasoft@gmail.com</p>
                </div>
              </div>
              <div class="contact_right">
                <div class="phone_img">
                  <img src="../assets/contact/phone.svg" alt="" />
                </div>
                <div class="contact-with-us">
                  <h6 data-aos="fade-right">Contact Us</h6>
                  <p data-aos="fade-left">+ 855 12346789</p>
                </div>
              </div>
            </div>
          </div>
          <div class="office-img">
            <!-- <img src="@/assets/university/contact_form.png" alt="" /> -->
            <img src="@/assets/contact/image 18.png" alt="" data-aos="fade-left"/>
          </div>
        </div>
      </div>
      <!-- <div class="ask-question mt-5">
          <h1 class="title" style="display: flex; justify-content: center; padding: 50px">
            Frequently Asked Questions
          </h1>
          <div class="asking-side" style="padding-left: 30px">
            <div class="ask-img">
              <img src="../assets/contact/image 19.png" alt="" />
            </div>
            <div class="dropdown">
              <div class="dropdown1">
                <div class="dropdown-qa" @click="toggleDropdown(1)">
                  <h4 class="dropbtn">How do I sign up for an account?</h4>
                  <i class="fa fa-caret-down"></i>
                </div>
                <div class="drop-text" v-show="openDropdown === 1">
                  <span>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Totam provident architecto ea voluptatibus laborum eius
                    doloremque possimus rem perspiciatis tenetur.
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Totam provident architecto ea voluptatibus laborum eius
                    doloremque possimus rem perspiciatis tenetur.
                  </span>
                </div>
              </div>
              <hr />
              <div class="dropdown2">
                <div class="dropdown-qa" @click="toggleDropdown(2)">
                  <h4 class="dropbtn">Can I transfer funds to accounts outside of this bank?</h4>
                  <i class="fa fa-caret-down"></i>
                </div>
                <div class="drop-text" v-show="openDropdown === 2">
                  <span>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Totam provident architecto ea voluptatibus laborum eius
                    doloremque possimus rem perspiciatis tenetur.
                  </span>
                </div>
              </div>
              <hr />
              <div class="dropdown3">
                <div class="dropdown-qa" @click="toggleDropdown(3)">
                  <h4 class="dropbtn">Can I set up personalized alerts for my account?</h4>
                  <i class="fa fa-caret-down"></i>
                </div>
                <div class="drop-text" v-show="openDropdown === 3">
                  <span>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Totam provident architecto ea voluptatibus laborum eius
                    doloremque possimus rem perspiciatis tenetur.
                  </span>
                </div>
              </div>
              <hr />
              <div class="dropdown4">
                <div class="dropdown-qa" @click="toggleDropdown(4)">
                  <h4 class="dropbtn">Can I transfer funds to accounts outside of this bank?</h4>
                  <i class="fa fa-caret-down"></i>
                </div>
                <div class="drop-text" v-show="openDropdown === 4">
                  <span>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Totam provident architecto ea voluptatibus laborum eius
                    doloremque possimus rem perspiciatis tenetur.
                  </span>
                </div>
              </div>
              <hr />
              <div class="dropdown5">
                <div class="dropdown-qa" @click="toggleDropdown(5)">
                  <h4 class="dropbtn">Can I transfer funds to accounts outside of this bank?</h4>
                  <i class="fa fa-caret-down"></i>
                </div>
                <div class="drop-text" v-show="openDropdown === 5">
                  <span>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Totam provident architecto ea voluptatibus laborum eius
                    doloremque possimus rem perspiciatis tenetur.
                  </span>
                </div>
              </div>
              <hr />
              <div class="dropdown5">
                <div class="dropdown-qa" @click="toggleDropdown(6)">
                  <h4 class="dropbtn">Can I transfer funds to accounts outside of this bank?</h4>
                  <i class="fa fa-caret-down"></i>
                </div>
                <div class="drop-text" v-show="openDropdown === 6">
                  <span>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Totam provident architecto ea voluptatibus laborum eius
                    doloremque possimus rem perspiciatis tenetur.
                  </span>
                </div>
              </div>
              <hr />
              <div class="dropdown5">
                <div class="dropdown-qa" @click="toggleDropdown(7)">
                  <h4 class="dropbtn">Can I transfer funds to accounts outside of this bank?</h4>
                  <i class="fa fa-caret-down"></i>
                </div>
                <div class="drop-text" v-show="openDropdown === 7">
                  <span>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Totam provident architecto ea voluptatibus laborum eius
                    doloremque possimus rem perspiciatis tenetur.
                  </span>
                </div>
              </div>
              <hr />
              <div class="dropdown5">
                <div class="dropdown-qa" @click="toggleDropdown(8)">
                  <h4 class="dropbtn">Can I transfer funds to accounts outside of this bank?</h4>
                  <i class="fa fa-caret-down"></i>
                </div>
                <div class="drop-text" v-show="openDropdown === 8">
                  <span>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit.
                    Totam provident architecto ea voluptatibus laborum eius
                    doloremque possimus rem perspiciatis tenetur.
                  </span>
                </div>
              </div>
            </div>
          </div>
        </div> -->
    </div>
    <FooTer></FooTer>
  </div>
</template>
<script>
import NavBar from "@/components/NavBar.vue";
import FooTer from "@/components/FooTer.vue";

export default {
  components: {
    NavBar,
    FooTer,
  },
  data() {
    return {
      openDropdown: null,
    };
  },
  methods: {
    toggleDropdown(index) {
      this.openDropdown = this.openDropdown === index ? null : index;
    },
  },
};
</script>
<style scoped>
.contact-us-page {
  background-color: #f8f7f5;
}
.contact {
  margin: 20px;
}
.title {
  margin-top: 130px;
  display: flex;
  justify-content: center;
  margin-bottom: 30px;
}
.sub-title {
  display: flex;
  justify-content: center;
  width: 50%;
  align-items: center;
  margin-left: 25%;
}
.form-contact {
  display: flex;
  justify-content: center;
  margin: 0px;
}
.row {
  display: flex;
  gap: 3px;
  background-color: #f8f7f5;
  width: 70%;
  height: 90vh;
  padding: 0 5% 0 5%;
  border-radius: 20px;
  border: 1px solid #3b53a4;
}
.row h1 {
  display: flex;
  justify-content: center;
  align-items: center;

  margin-top: 20px;
}
.full_name,
.mail_address {
  display: flex;
  width: 100%;
  justify-content: space-between;
}

.first_name,
.last_name,
.address,
.phone_number {
  width: 45%;
}
input {
  border: none;
  border-bottom: 1px solid grey;
}
label {
  font-weight: bold;
}

.office-info p {
  margin-top: 50px;
}
.office-info {
  margin-left: 30px;
  width: 40%;
}
.office-info h1,
.contact-with-us h6,
label,
.row h1{
  color: #0f58a8;
}
.contact-with-us p {
  margin-top: 5px;
}
.contact-us-section {
  background-image: url("@/assets/contact/banner-contact.svg");
  height: 70vh;
  background-position: center;
  background-repeat: no-repeat;
  color: white;
}
.submit {
  display: flex;
  justify-content: center;
}
.btn_submit {
  width: 100%;
  border: none;
  border-radius: 30px;
  height: 40px;
  background-color: #3b53a4;
  color: white;
}
.btn_submit:hover {
  filter: brightness(1.1);
  transition: filter 0.3s ease-in-out;
  transform: scale(1.01);
  cursor: pointer;
}
.hard-office {
  display: flex;
  margin-top: 200px;
  justify-content: space-between;
  padding-left: 30px;
}
.office-img {
  display: flex;
  width: 40%;
  height: 600px;
  margin-right: 70px;
  border-radius: 20px;
  background-position: center;
}
.office-img img{
  width: 100%;
  height: 100%;
  border-radius: 20px;
}
.office-contact {
  display: flex;
  justify-content: space-between;
}
.contact_left,
.contact_right {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: left;
  gap: 1rem;
}
.contact-with-us {
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.card-custom img {
  width: 30%;
  height: 80%;
  object-fit: cover;
  border-radius: 20px;
  background-repeat: no-repeat;
}

.contact-us-section {
  text-align: center;
  padding: 50px 0;
}

.contact-us-title {
  font-size: 4rem;
  font-weight: bold;
  position: relative;
  color: rgb(6, 6, 134);
  margin-top: 100px;
}

.contact-us-title::before {
  content: "GET IN TOUCH";
  font-size: 6rem;
  position: absolute;
  top: -65px;
  left: 50%;
  transform: translateX(-50%);
  color: rgba(9, 103, 226, 0.144);
}

.breadcrumb {
  display: flex;
  justify-content: center;
  margin-top: 30px;
}

.container {
  background-color: rgb(6, 45, 116);
  padding: 20px;
  width: 100%;
  height: 200px;
  margin-right: -70px;
  margin-top: 20px;
  border-top-left-radius: 30px;
  border-bottom-left-radius: 100px;
}

.asking-side {
  display: flex;
}

.ask-img img {
  width: 420px;
  height: 500px;
  border-radius: 20px;
  background-repeat: no-repeat;
  background-position: center;
}

.dropdown {
  display: flex;
  flex-direction: column;
  margin: 0px 20px 0px 50px;
  height: 500px;
  overflow-y: auto;
  scrollbar-width: none;
  -ms-overflow-style: none;
  overflow-x: hidden;
}

.dropdown-qa {
  display: flex;
  justify-content: space-between;
  cursor: pointer;
  width: 930px;
}

.drop-text {
  width: 90%;
}
@media (min-width: 768px) and (max-width: 1024px) {
  .contact-us-section {
    display: flex;
    flex-direction: column;
    margin-top: 70px;
    margin-bottom: 50px;
    height: 30vh;
    border-radius: 20px;
    background-position: center;
    background-repeat: no-repeat;
  }
  .title {
    display: flex;
    margin-top: 10px;
    justify-content: center;
    margin-bottom: 30px;
  }
  .sub-title {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 50%;
    margin-left: 180px;
  }
  .row {
    flex-direction: column;
    gap: 10px;
    background-color: #f8f7f5;
    width: 100%;
    height: 50vh;
    padding: 0 5% 0 5%;
    border-radius: 20px;
    border: 1px solid #3b53a4;
  }
  .hard-office {
    flex-direction: column;
    margin-top: 100px;
    padding-left: 0;
  }
  .office-info {
    margin-left: 0;
    width: 100%;
  }
  .office-img {
    width: 100%;
    height: 400px;
  }
  .office-img img {
    width: 100%;
    height: 100%;
  }
}
@media (min-width: 428px) and (max-width: 767px) {
  .contact-us-section {
    display: flex;
    flex-direction: column;
    margin-top: 70px;
    margin-bottom: 20px;
    height: 25vh;
    border-radius: 20px;
    background-position: center;
    background-repeat: no-repeat;
  }
  .email_img,
  .phone_img{
    margin-top: -10px;
  }
  .title {
    margin-top: 0px;
    display: flex;
    justify-content: center;
    font-size: 1.5rem;
    margin-bottom: 20px;
  }
  .sub-title {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 90%;
    margin-left: 20px;
    margin-bottom: 10px;
    font-size: 0.90rem;
  }
  .row {
    flex-direction: column;
    gap: 10px;
    background-color: #f8f7f5;
    width: 100%;
    height: auto;

    padding: 0 5% 5% 5%;
    border-radius: 20px;
    border: 1px solid #3b53a4;
  }
  .full_name,
  .mail_address{
    display: flex;
    flex-direction: column;
  }
  .first_name,
  .last_name,
  .address,
  .phone_number {
    width: 100%;
  }
  .hard-office {
    flex-direction: column;
    margin-top: 100px;
    padding-left: 0;
  }
  .office-info {
    margin-left: 0;
    width: 100%;
  }
  .office-img {
    width: 100%;
    height: 250px;
  }
  .office-img img {
    width: 100%;
    height: 100%;
  }
  .office-contact{
    display: flex;
    flex-direction: column;
    margin-bottom: 20px;
    gap: 5px;
    margin-left: 0;
    align-items: start;
  }
  
}
</style>
