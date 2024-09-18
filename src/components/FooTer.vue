<template>
  <footer class="footer">
    <div class="footer-content">
      <div class="footer_logo">
        <img src="../assets/logo/Logo_white.svg" alt="Logo" class="logo" data-aos="fade-right"/>
        <span data-aos="fade-left">
          Vectorasoft is a leading provider of business and educational software
          solutions, dedicated to transforming the way organizations operate.
        </span>
      </div>
      <div class="footer-links">
        <div class="footer-column">
          <h4 data-aos="fade-right">Other</h4>
          <ul data-aos="fade-left">
            <li><router-link to="/">Home</router-link></li>
            <li><router-link to="/product">Product</router-link></li>
            <li><router-link to="/about">About Us</router-link></li>
          </ul>
        </div>
        <div class="footer-address">
          <h4 data-aos="fade-right">Address</h4>
          <div class="address_info">
            <i class="fa fa-map-marker" data-aos="fade-right"></i>
            <span data-aos="fade-left">
              AP-1151, Aphivath BLV, Dermkor, Chongva, Chroy Changva. <br />
              Phnom Penh, Cambodia
            </span>
          </div>
        </div>
        <div class="footer_contact">
          <h4 data-aos="fade-right">Contact Us</h4>
          <div class="email">
            <i class="fa fa-envelope" data-aos="fade-right"></i>
            <span data-aos="fade-left">Email: vectorasoft@gmail.com</span>
          </div>
          <div class="phone">
            <i class="fa fa-phone" data-aos="fade-right"></i>
            <span data-aos="fade-left">Tel: 012 528 131</span>
          </div>
          <div class="search_box">
            <input class="search_email" type="text" placeholder="Email" v-model="email" data-aos="fade-left"/>
            <input class="search_tel" type="text" placeholder="Phone" v-model="phone" data-aos="fade-right"/>
          </div>
          <button class="send" @click="sendContactInfo" data-aos="fade-left">
            Send <i class="fa fa-paper-plane"></i>
          </button>
        </div>
      </div>
    </div>
    <div class="footer-bottom">
      <p>Copyright @Vectorasoft | Designed by Vectorasoft</p>
      <div class="social-icons">
        <a href="https://www.facebook.com/" class="social-icon">
          <i class="fab fa-facebook-f"></i>
        </a>
        <a href="https://www.linkedin.com" class="social-icon">
          <i class="fab fa-linkedin-in"></i>
        </a>
        <a href="https://t.me/" class="social-icon">
          <i class="fab fa-telegram-plane"></i>
        </a>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooTer",
  data() {
    return {
      email: '',
      phone: ''
    };
  },
  methods: {
    sendContactInfo() {
      // Validate email and phone
      if (this.email === '' || this.phone === '') {
        alert('Please fill out both the email and phone fields.');
        return;
      }

      // Example of a simple alert to simulate sending data
      alert(`Contact info sent: Email: ${this.email}, Phone: ${this.phone}`);

      // Clear the form fields
      this.email = '';
      this.phone = '';
    }
  }
};
</script>

<style scoped>
.footer {
  background-color: rgb(6, 45, 116);
  color: #fff;
  padding: 50px;
  border-top-left-radius: 30px;
  border-top-right-radius: 30px;
  margin-top: 80px;
}

.footer-content {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
}

.footer_logo {
  display: flex;
  flex-direction: column;
  text-align: left;
  width: 25%;
  margin-bottom: 20px;
}

.footer_logo .logo {
  width: 250px;
  margin-bottom: 10px;
}
.footer-links {
  margin-top: 5px;
  display: flex;
  justify-content: space-around;
  flex: 1;
  gap: 5px;
  margin-left: 50px;
}

.footer-column {
  display: flex;
  flex-direction: column;
  min-width: 150px;
}
.footer-address {
  display: flex;
  flex-direction: column;
  gap: 5px;
}
.address_info {
  display: flex;
  width: 70%;
  gap: 1rem;
}
.footer_contact {
  display: flex;
  flex-direction: column;
  gap: 5px;
  width: 50%;
}
.email,
.phone {

  display: flex;
  width: 100%;
  gap: 1rem;
  align-items: center;
  font-size: 16px;
}
.search_box{
  display: flex;
  flex-direction: column;
  margin-top: 10px;
}
.search_email,
.search_tel {
  width: 100%;
  padding: 8px 15px;
  border: 1px solid #ccc;
  border-radius: 30px;
  margin-bottom: 15px;
  transition: border-color 0.3s ease, box-shadow 0.3s ease;
  font-size: 16px;
  background-color: #f4f4f4;
  color: #333;
}

.search_email::placeholder,
.search_tel::placeholder {
  color: #aaa;
}

.search_email:focus,
.search_tel:focus {
  border-color: #1275B1;
  box-shadow: 0 0 8px rgba(247, 189, 29, 0.5);
  outline: none;
  background-color: #fff;
}
.send {
  display: flex;
  background-color: #f7bd1d;
  color: #fff;
  font-weight: bold;
  justify-content: center;
  align-items: center;
  width: 30%;
  border: none;
  border-radius: 30px;
  gap: 1rem;
  padding: 8px 15px;
  cursor: pointer;
}

.footer-column ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.footer-column ul li {
  margin-bottom: 8px;
}

.footer-column ul li a {
  color: #fff;
  text-decoration: none;
}

.footer-bottom {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 20px;
  border-top: 1px solid #ffffff;
  padding-top: 10px;
}

.footer-bottom p {
  margin: 0;
  font-size: 12px;
}

.social-icons {
  display: flex;
  justify-content: flex-start;
  align-items: center;
}

.social-icon {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background: linear-gradient(180deg, #1275B1 0%, #1275B1 100%);
  color: white;
  margin-right: 10px;
}
/* Add these styles to your existing CSS */

/* Hide the 'Other' footer column on tablets (768px to 1024px) */
@media (max-width: 1024px) and (min-width: 768px) {
  .footer-content{
    display: flex;
    justify-content: space-between;
    gap: 0;
    width: 100%;
  }
  .footer-column {
    display: none;
  }
  .footer_logo{
    width: 33.33%;
    margin-bottom: 0;
  }
  .footer_logo .logo{
    width: 80%;
    margin-bottom: 10px;
  }
  .send{
    width: 50%;
    margin-left: 0;
  }
}

/* Hide the entire footer on phones (max-width: 767px) */
@media (max-width: 767px) {
  .footer {
    display: none;
  }
}

</style>
