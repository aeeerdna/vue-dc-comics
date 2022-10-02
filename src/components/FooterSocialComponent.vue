<template>
  <div class="social">
    <!-- Social area -->
    <div class="container">
      <!-- Pulsante Sign-up -->
      <div class="btn-sign">
        <button>Sign-up now!!</button>
      </div>

      <!-- Parte social, seguici! -->
      <div class="follow-us">
        <p>Follow us</p>
        <div class="img-container">
          <img src="../assets/img/footer-facebook.png" alt="Facebook" />
          <img src="../assets/img/footer-twitter.png" alt="Twitter" />
          <img src="../assets/img/footer-youtube.png" alt="YouTube" />
          <img src="../assets/img/footer-pinterest.png" alt="Pinterest" />
          <img src="../assets/img/footer-periscope.png" alt="Periscope" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import "../styles/variable.scss";

.social {
  background-color: $bg-footer;
  padding-top: 25px;
  padding-bottom: 25px;
}

.container {
  display: flex;
  justify-content: space-between;
}

.btn-sign {
  display: flex;
  align-items: center;

  button {
    color: $txt-main;
    background-color: $bg-footer;
    border: 2px $bg-dc-blue solid;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 1.2rem;
    padding: 15px 20px;
  }
}
.follow-us {
  display: flex;
  align-items: center;

  p {
    padding-right: 20px;
    text-transform: uppercase;
    color: $bg-dc-blue;
    font-weight: bold;
    font-size: 1.2rem;
  }

  .img-container {
    display: flex;

    img {
      padding-right: 5px;
    }
  }
}
</style>
