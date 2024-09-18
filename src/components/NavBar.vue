<template>
  <nav class="navbar navbar-expand-lg navbar-light">
    <div class="container-fluid">
      <img src="../assets/logo/Logo_company.png" alt="Logo" class="logo" />
      <ul class="nav-links">
        <li><router-link to="/">HOME</router-link></li>
        <li><router-link to="/product">PRODUCTS</router-link></li>
        <!-- <li><router-link to="/service">SERVICES</router-link></li> -->
        <li><router-link to="/about">ABOUT US</router-link></li>
      </ul>
      <div class="btn-class">
        <button @click="navigateToRoute" type="button" class="btn btn-lg text-white">
          CONTACT US
        </button>
      </div>
      <button class="menu-icon" @click="toggleMenu">
        <span class="menu-icon-bar"></span>
        <span class="menu-icon-bar"></span>
        <span class="menu-icon-bar"></span>
      </button>
      <ul class="mobile-nav-links" :class="{ 'show': isMenuOpen }">
        <li><router-link to="/">HOME</router-link></li>
        <li><router-link to="/product">PRODUCTS</router-link></li>
        <!-- <li><router-link to="/service">SERVICES</router-link></li> -->
        <li><router-link to="/about">ABOUT US</router-link></li>
        <li>
          <button @click="navigateToRoute" type="button" class="btn">
            CONTACT US
          </button>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    navigateToRoute() {
      this.$router.push('/contact');
    },
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
  },
};
</script>

<style scoped>
.navbar {
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 1000;
  background: #ffffff;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.logo {
  cursor: pointer;
  width: 20%;
  margin-left: 50px;
}

.nav-links {
  list-style: none;
  display: flex;
  flex-grow: 1; 
  justify-content: center; 
  margin: 0; 
  padding: 0;
}

.nav-links li {
  margin: 0 80px; 
}

nav a {
  text-decoration: none;
  color: black;
}

nav a.router-link-active {
  font-weight: bold; 
  color: #3B53A4;
}

.btn-class {
  margin-right: 50px;
}

.btn {
  border-radius: 32px;
  background-color: #3b53a4;
  color: white; 
}

/* Mobile menu styles */
.menu-icon {
  display: none;
  border: none;
  background: none;
  cursor: pointer;
  padding: 10px;
}

.menu-icon-bar {
  display: block;
  width: 25px;
  height: 3px;
  background-color: #3b53a4;
  margin: 5px 0;
}

/* Mobile menu links */
.mobile-nav-links {
  list-style: none;
  display: none;
  flex-direction: column;
  position: absolute;
  top: 60px;
  right: 0;
  background: white;
  width: 100%;
  text-align: center;
  padding: 10px 0;
  border: 1px solid #ddd;
}

.mobile-nav-links li {
  margin: 10px 0;
}

/* Show menu on mobile */
.mobile-nav-links.show {
  display: flex;
}

@media (max-width: 768px) {
  .logo {
    width: 30%;
    margin-left: 10px;
  }
  .nav-links {
    display: none;
  }
  .btn-class {
    display: none;
  }
  .menu-icon {
    display: block;
  }
  .btn{
    margin-right: 0;
    margin-bottom: 10px;
    border: none;
    background-color: white;
    color: black;
  }
}

@media (min-width: 769px) {
  .mobile-nav-links {
    display: none;
  }
}
</style>
