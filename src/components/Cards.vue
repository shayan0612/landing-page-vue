<template>
  <div class="main-container">
    <div class="heading">
      <h1>Coverage Forms</h1>
    </div>
    <div class="cards">
      <div class="main-card" v-for="(card, index) in cards" :key="index">
        <div class="flexbox">
          <div class="image">
            <img :src="card.cardImg" alt="" />
          </div>
          <div class="content" :style="card.background">
            <h3>{{ card.cardTitle }}</h3>
            <p>{{ card.cardContent }}</p>
          </div>
        </div>
      </div>

      <b-button class="btn-cards">Educational Center</b-button>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardComponent",
  data() {
    return {
      cards: [
        {
          cardId: 1,
          cardImg: require("../assets/images/first-.png"),
          cardTitle: "General Liablity",
          cardContent: "What every brand must have",
          background:
            "background: linear-gradient(92.68deg, #fdc0e4 0%, #f2fec7 100.25%)",
        },
        {
          cardId: 2,
          cardImg: require("../assets/images/second-icon.png"),
          cardTitle: "Workers Comp",
          cardContent: "Require if you have employes",
          background:
            "background: linear-gradient(92.68deg, #9bfce6 0%, #e3fd83 100.25%)",
        },
        {
          cardId: 3,
          cardImg: require("../assets/images/third.png"),
          cardTitle: "Cyber Liablity",
          cardContent: "Do you sell your product online?",
          background:
            "background: linear-gradient(92.68deg, #c7c9fd 0%, #ffaee8 100.25%)",
        },
        {
          cardId: 4,
          cardImg: require("../assets/images/fourth.png"),
          cardTitle: "Product Recall",
          cardContent: "Can you afford a large product recall",
          background:
            "background:linear-gradient(92.68deg, #9bfce6 0%, #fed0eb 100.25%)",
        },
      ],
    };
  },
};
</script>

<style scoped>
.heading {
  text-align: center;
  margin-top: 10px;
  margin-bottom: 10px;  
}
.cards {
  background: linear-gradient(180deg, #ffffff 0%, #fdc0e4 100%);
  padding: 5rem;
}
.main-card {
  padding: 10px 4rem;
}
.card-1 {
  display: flex;
  align-items: center;
}
.content {
  /* background: linear-gradient(92.68deg, #fdc0e4 0%, #f2fec7 100.25%); */
  width: 989px;
  padding: 2rem 2rem;
  margin-left: 3rem;
  border: 1px solid black;
  border-radius: 24px;
}
.content2 {
  background: linear-gradient(92.68deg, #9bfce6 0%, #e3fd83 100.25%);

  width: 989px;
  padding: 2rem 2rem;
  margin-left: 3rem;
  border: 1px solid black;
  border-radius: 24px;
}
.content3 {
  background: linear-gradient(92.68deg, #c7c9fd 0%, #ffaee8 100.25%);

  width: 989px;
  padding: 2rem 2rem;
  margin-left: 3rem;
  border: 1px solid black;
  border-radius: 24px;
}
.content4 {
  background: linear-gradient(92.68deg, #9bfce6 0%, #fed0eb 100.25%);
  width: 100%;
  padding: 2rem 2rem;
  margin-left: 3rem;
  border: 1px solid black;
  border-radius: 24px;
}

.content h3 {
  color: #a21081;
  font-size: 40px;
  font-weight: 700;
  line-height: 30px;
}
.content p {
  font-size: 25px;
  font-weight: 700;
  line-height: 30px;
}
.content2 h3 {
  color: #a21081;
  font-size: 40px;
  font-weight: 700;
  line-height: 30px;
}
.content2 p {
  font-size: 20px;
  font-weight: 700;
  line-height: 30px;
}
.content3 h3 {
  color: #a21081;
  font-size: 40px;
  font-weight: 700;
  line-height: 30px;
}
.content3 p {
  font-size: 25px;
  font-weight: 700;
  line-height: 30px;
}
.content4 h3 {
  color: #a21081;
  font-size: 40px;
  font-weight: 700;
  line-height: 30px;
}
.content4 p {
  font-size: 25px;
  font-weight: 700;
  line-height: 30px;
}

.image img {
  width: 15rem;
  height: 10rem;
}
.btn-cards {
  border-radius: 1.25rem;
  color: #fd4cb7;
  background: #e3fd83;
  border: none;
  text-align: center;
  display: flex;
  margin: 4rem auto;
  padding: 8px;
}
.flexbox {
  display: flex;
}
@media (max-width: 992px) {
  .flexbox {
    display: block;
  }
  .content {
    margin-left: 0;
    width: 100%;
  }
  .image {
    text-align: center;
    margin: 20px 0;
  }
}
@media (max-width: 768px) {
  .content h3 {
    font-size: 30px;
  }
  .content p {
    font-size: 20px;
  }
  .content {
    width: 100%;
  }
  .cards {
    padding: 2rem;
  }
}
@media (max-width: 600px) {
  .content h3 {
    font-size: 25px;
  }
  .content p {
    font-size: 15px;
  }
  .image img {
    width: 10rem;
    height: 6rem;
  }
}
</style>
