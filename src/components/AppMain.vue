<script>
import AppCard from "./AppCard.vue";
export default {
  data() {
    return {
      books: [
        {
          thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },

  components: {
    AppCard,
  },
};
</script>

<template>
  <div class="jumbo"></div>
  <div class="containerCard">
    <button class="series">Current series</button>
    <AppCard
      v-for="book in books"
      :key="book.type"
      :thumb="book.thumb"
      :series="book.series"
    >
    </AppCard>
    <button class="load">Load More</button>
  </div>
  <div class="icons">
    <div class="iconMenu">
      <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
      <p>DIGITAL COMICS</p>
    </div>
    <div class="iconMenu">
      <img src="../assets/img/buy-comics-merchandise.png" alt="" />
      <p>MERCHANDISE</p>
    </div>
    <div class="iconMenu">
      <img src="../assets/img/buy-comics-subscriptions.png" alt="" />
      <p>SUBSCRIPTION</p>
    </div>
    <div class="iconMenu">
      <img src="../assets/img/buy-comics-shop-locator.png" alt="" />
      <p>COMIC SHOP LOCATOR</p>
    </div>
    <div class="iconMenu">
      <img src="../assets/img/buy-dc-power-visa.svg" alt="" />
      <p>DC POWER VISA</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/style/partial/variables" as *;
.containerCard {
  max-width: 1250px;
  padding-top: 20px;
  position: relative;
  display: flex;
  margin: auto;
  justify-content: center;
  flex-wrap: wrap;
  .series {
    @include buttonMain;

    position: absolute;
    top: -30px;
    left: -10px;
  }
}
.jumbo {
  background-size: 100%;
  background-position-x: center;
  height: 350px;
  background-image: url(../assets/img/jumbotron.jpg);
}

.load {
  margin: 30px;
  @include buttonMain;
}
.icons {
  background-color: #0c7cec;
  display: flex;
  justify-content: center;
  margin: auto;
  align-items: center;
  height: 150px;
}
.iconMenu {
  display: flex;
  align-items: center;
  margin: 20px;
  p {
    color: white;
    margin-left: 10px;
  }
}
img {
  width: 45px;
  height: 55px;
}
</style>
