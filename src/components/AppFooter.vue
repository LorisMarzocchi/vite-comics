<script>
export default {};
</script>

<template>
  <footer>
    <div class="container">
      <div class="linkContainer">
        <ul>
          <li class="linkArea">DC COMICS</li>
          <li>Charaters</li>
          <li>Comics</li>
          <li>Movies</li>
          <li>TV</li>
          <li>Games</li>
          <li>Videos</li>
          <li>News</li>
          <li class="linkArea">SHOP</li>
          <li>Shop DC</li>
          <li>Shop DC Collectibles</li>
        </ul>

        <ul>
          <li class="linkArea">DC</li>
          <li>Terms Of Use</li>
          <li>Privacy policy (New)</li>
          <li>Ad Choices</li>
          <li>Advertising</li>
          <li>Jobs</li>
          <li>Subscriptions</li>
          <li>Talent Workshops</li>
          <li>CPSC Certificates</li>
          <li>Ratings</li>
          <li>Shop Help</li>
          <li>Contact Us</li>
        </ul>

        <ul>
          <li class="linkArea">SITES</li>
          <li>DC</li>
          <li>MAD Magazine</li>
          <li>DC Kids</li>
          <li>DC Universe</li>
          <li>DC Power Visa</li>
        </ul>
      </div>
      <div class="logoBg">
        <!-- <img src="../assets/img/dc-logo-bg.png" alt="" /> -->
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scope>
footer {
  color: #959595;
  background-image: url(../assets/img/footer-bg.jpg);
  height: 400px;
  display: flex;
  align-items: center;
  justify-content: space-around;
}
.linkContainer {
  width: 50%;
  margin-top: 55px;
  padding-right: 80px;
  display: flex;
  justify-content: space-between;
  li {
    list-style: none;
  }
  .linkArea {
    color: white;
  }
}
.container {
  width: 1250px;
  margin: auto;
  display: flex;
  justify-content: center;
}
.logoBg {
  background-image: url(../assets/img/dc-logo-bg.png);
  height: 400px;
  background-repeat: no-repeat;
  background-position: center;
  width: 50%;
  align-items: center;
}
</style>
