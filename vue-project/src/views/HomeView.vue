<template>
  <div class="hewwo">
    <h1>hello</h1>
    <div class="items">
      <h2 v-for="star in stars" :key="star.name">{{ star.name }}</h2>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      stars: [
        { name: "Do Ha", lastName: "Bak", group: "K", height: "180", pic: "" },
        { name: "Woong Ki", lastName: "Cha", group: "K", height: "", pic: "" },
        { name: "Woo Jin", lastName: "Choi", group: "K", height: "", pic: "" },
        { name: "Yu Jin", lastName: "Han", group: "K", height: "", pic: "" },
        { name: "I Chan", lastName: "Jeong", group: "K", height: "", pic: "" },
        { name: "Yun Seo", lastName: "Ji", group: "K", height: "", pic: "" },
        { name: "Min Gyu", lastName: "Jung", group: "K", height: "", pic: "" },
        { name: "Gyu Vin", lastName: "Kim", group: "K", height: "", pic: "" },
        { name: "Ji Woong", lastName: "Kim", group: "K", height: "", pic: "" },
        { name: "Tae Rae", lastName: "Kim", group: "K", height: "", pic: "" },
        { name: "Jun Hyeon", lastName: "Kum", group: "K", height: "", pic: "" },
        { name: "Da Eul", lastName: "Lee", group: "K", height: "", pic: "" },
        { name: "Dong Gun", lastName: "Lee", group: "K", height: "", pic: "" },
        { name: "Dong Yeol", lastName: "Lee", group: "K", height: "", pic: "" },
        { name: "Hoe Taek", lastName: "Lee", group: "K", height: "", pic: "" },
        { name: "Ye Dam", lastName: "Lee", group: "K", height: "", pic: "" },
        { name: "Jun Seo", lastName: "Lim", group: "K", height: "", pic: "" },
        { name: "Jung Hyun", lastName: "Mun", group: "K", height: "", pic: "" },
        { name: "Sung Min", lastName: "Oh", group: "K", height: "", pic: "" },
        { name: "Gun Wook", lastName: "Park", group: "K", height: "", pic: "" },
        { name: "Han Bin", lastName: "Park", group: "K", height: "", pic: "" },
        {
          name: "Hyun Been",
          lastName: "Park",
          group: "K",
          height: "",
          pic: "",
        },
        { name: "Ji Hoo", lastName: "Park", group: "K", height: "", pic: "" },
      ],
    };
  },
  methods: {},
};
</script>

<style scoped>
.hewwo {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  flex-direction: row;
  padding: 2.5rem;
  text-align: center;
}
.items {
  flex: 0 0 23.5%;
  width: 32vw;
  margin: 25px auto;
  background-color: red;
  align-content: center;
  border: solid white;
  border-radius: 25px;
}
</style>
