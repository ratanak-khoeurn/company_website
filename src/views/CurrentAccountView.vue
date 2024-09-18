<template>
  <NavBar />
  <div class="current-account" style="background-color: #f8f7f5">
    <div class="account-img">
      <div class="all-current-title" style="display: flex">
        <div class="current-title">
          <h1>
            Meet the bank <br />
            of the future
          </h1>
        </div>
        <div class="account-info">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
            eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim
            ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut .
          </p>
          <button
          class="get_start"
            type="button"
            style="
              background-color: #3b53a4;
              border: none;
              border-radius: 30px;
              color: white;
              width: 150px;
              padding: 10px;
            "
          >
            Get Started
          </button>
        </div>
      </div>

      <div
        class="manage"
        style="
          display: flex;
          flex-direction: column;
          align-items: end;
          margin-top: 50px;
        "
      >
        <h1>99%</h1>
        <p>Customer satisfation</p>
        <h1>800k</h1>
        <p>customers</p>
        <h1>250B</h1>
        <p>Money Managed</p>
      </div>
    </div>

    <div class="all-info ps-5 py-5">
      <div class="a-title">
        <h1>Browse our set of banking <br />services offering</h1>
      </div>
      <div class="a-about" style="display: flex; margin-top: 50px">
        <div class="a-title">
          <h2>Current Account</h2>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere quae
            quaerat iste in nesciunt ducimus magni ipsam numquam qui, corporis
            ad odit fugit voluptates. Labore quos eos natus reiciendis placeat.
          </p>
        </div>
        <div class="a-img" style="margin-right: 50px">
          <img src="../assets/image/current-img.png" alt="" />
        </div>
      </div>
    </div>
    <FooTer></FooTer>
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from "@/components/NavBar.vue";
import FooTer from "@/components/FooTer.vue";

export default {
  name: "CurrentAccount",
  components: {
    NavBar,
    FooTer,
  },
};
</script>

<style>
.account-img {
  background-image: url("@/assets/image/bg-current.png");
  margin-top: 74px;
  height: 640px;
  box-shadow: inset 0 0 285px rgb(0, 0, 0);
  background-position: center;
  background-repeat: no-repeat;
  background-size: 100% 100%;
  padding: 10% 5%;
  color: white;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.account-info {
  width: 50%;
  margin-left: 30%;
}
.a-title p {
  width: 70%;
}
.get_start:hover{
  filter: brightness(1.2);
  transition: filter 0.3s ease-in-out;
  transition: transform 0.3s ease-in-out;
  transform: scale(1.05);
  cursor: pointer;
}
</style>
