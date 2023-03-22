<template>
  <div class="parent">
    <div>
      <TheCards
        v-for="star in stars"
        :key="star.name"
        :name="star.name"
        :lastname="star.lastName"
        :image="star.img"
        class="cards"
      />
    </div>
  </div>
</template>

<script>
import TheCards from "../components/TheCards.vue";

export default {
  name: "ProductsList",
  components: { TheCards },
  data() {
    return {
      selected: "",
      stars: [
        {
          name: "Do Ha",
          lastName: "Bak",
          group: "K",
          img: "",
        },
        { name: "Woong Ki", lastName: "Cha", group: "K", img: "" },
        { name: "Woo Jin", lastName: "Choi", group: "K", img: "" },
        { name: "Yu Jin", lastName: "Han", group: "K", img: "" },
        { name: "I Chan", lastName: "Jeong", group: "K", img: "" },
        { name: "Yun Seo", lastName: "Ji", group: "K", img: "" },
        { name: "Min Gyu", lastName: "Jung", group: "K", img: "" },
        { name: "Gyu Vin", lastName: "Kim", group: "K", img: "" },
        { name: "Ji Woong", lastName: "Kim", group: "K", img: "" },
        { name: "Tae Rae", lastName: "Kim", group: "K", img: "" },
        { name: "Jun Hyeon", lastName: "Kum", group: "K", img: "" },
        { name: "Da Eul", lastName: "Lee", group: "K", img: "" },
        { name: "Dong Gun", lastName: "Lee", group: "K", img: "" },
        { name: "Dong Yeol", lastName: "Lee", group: "K", img: "" },
        { name: "Hoe Taek", lastName: "Lee", group: "K", img: "" },
        { name: "Ye Dam", lastName: "Lee", group: "K", img: "" },
        { name: "Jun Seo", lastName: "Lim", group: "K", img: "" },
        { name: "Jung Hyun", lastName: "Mun", group: "K", img: "" },
        { name: "Sung Min", lastName: "Oh", group: "K", img: "" },
        { name: "Gun Wook", lastName: "Park", group: "K", img: "" },
        { name: "Han Bin", lastName: "Park", group: "K", img: "" },
        {
          name: "Hyun Been",
          lastName: "Park",
          group: "K",
          img: "",
        },

        { name: "Ji Hoo", lastName: "Park", group: "K", img: "" },
        { name: "Won", lastName: "Seo", group: "K", img: "" },
        { name: "Han Bin", lastName: "Sung", group: "K", img: "" },
        { name: "Seung Eon", lastName: "Yoo", group: "K", img: "" },
      ],
    };
  },
  methods: {},
};
</script>

<style scoped>
.cards {
  flex: 0 0 23.5%;
  width: 32vw;
  margin: 25px auto;
  background-color: red;
  align-content: center;
  border: solid white;
  border-radius: 25px;
}

.parent {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  flex-direction: row;
  padding: 2.5rem;
  text-align: center;
}

.img {
  width: 2px;
}
</style>
