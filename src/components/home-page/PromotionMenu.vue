<template>
  <div class="promotions">
    <div class="btn-promotion">
      <button type="button" class="btn btn-dark" style="
            border-radius: 39px;
            margin-left: 80px;
            margin-top: 80px;
            font-size: 30px;
          ">
        Our Team
      </button>
      <hr />
    </div>
    <div class="card-container">
      <div class="card">
        <div class="card_img">
          <img class="activator" src="@/assets/image/hr.png" alt="ChrisopherLue" />
        </div>
        <div class="card-content">
          <h4 class="card-title">Chrisopher Lue</h4>
          <p>Deputy Chief Executive Officer</p>
          <hr />
        </div>
        <div class="social">
          <a href="#"><img src="@/assets/image/facebook.png" alt="facebook" /></a>
          <a href="#"><img src="@/assets/image/linkedin.png" alt="linkedIn" /></a>
          <a href="#"><img src="@/assets/image/telegram.png" alt="telegram" /></a>
        </div>
      </div>

      <div class="card">
        <div class="card_img">
          <img class="activator" src="@/assets/image/hr.png" alt="ChrisopherLue" />
        </div>
        <div class="card-content">
          <h4 class="card-title">Chrisopher Lue</h4>
          <p>Deputy Chief Executive Officer</p>
          <hr />
        </div>
        <div class="social">
          <a href="#"><img src="@/assets/image/facebook.png" alt="facebook" /></a>
          <a href="#"><img src="@/assets/image/linkedin.png" alt="linkedIn" /></a>
          <a href="#"><img src="@/assets/image/telegram.png" alt="telegram" /></a>
        </div>
      </div>
      
      <div class="card">
        <div class="card_img">
          <img class="activator" src="@/assets/image/hr.png" alt="ChrisopherLue" />
        </div>
        <div class="card-content">
          <h4 class="card-title">Chrisopher Lue</h4>
          <p>Deputy Chief Executive Officer</p>
          <hr />
        </div>
        <div class="social">
          <a href="#"><img src="@/assets/image/facebook.png" alt="facebook" /></a>
          <a href="#"><img src="@/assets/image/linkedin.png" alt="linkedIn" /></a>
          <a href="#"><img src="@/assets/image/telegram.png" alt="telegram" /></a>
        </div>
      </div>

    </div>

    <hr />
  </div>
</template>
<script>
export default {
  name: "PromotionsMenu",
  data() {
    return {
      promotions: [1, 2, 3, 4]
    };
  },
};
</script>

<style scoped>
.promotions {
  width: 100%;
}

.promotions hr {
  margin-top: 30px;
}

.btn-promotion hr {
  margin-left: 250px;
}


.card-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
}

.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  margin: 20px 0;
  height: 370px;
  width: 280px;
  border-radius: 20px;
  overflow: hidden;
  padding: 0;
  box-shadow: 0 2px 10px rgba(7, 21, 143, 0.1);
}
.card_img {
  width: 250px;
  height: 49%;
  background-repeat: no-repeat;
  display: flex;
  border-radius: 20px;
}

.card_img img {
  width: 100%;
  height: 100%;
}
</style>