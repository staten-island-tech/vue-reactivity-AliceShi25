<template>
  <div class="hewwo">
    <h1>hello</h1>
    <div class="items">
      <h2 v-for="star in stars" :key="star.name">
        {{ star.lastName }} {{ star.name }}
      </h2>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      stars: [
        { name: "Do Ha", lastName: "Bak", group: "K", pic: "" },
        { name: "Woong Ki", lastName: "Cha", group: "K", pic: "" },
        { name: "Woo Jin", lastName: "Choi", group: "K", pic: "" },
        { name: "Yu Jin", lastName: "Han", group: "K", pic: "" },
        { name: "I Chan", lastName: "Jeong", group: "K", pic: "" },
        { name: "Yun Seo", lastName: "Ji", group: "K", pic: "" },
        { name: "Min Gyu", lastName: "Jung", group: "K", pic: "" },
        { name: "Gyu Vin", lastName: "Kim", group: "K", pic: "" },
        { name: "Ji Woong", lastName: "Kim", group: "K", pic: "" },
        { name: "Tae Rae", lastName: "Kim", group: "K", pic: "" },
        { name: "Jun Hyeon", lastName: "Kum", group: "K", pic: "" },
        { name: "Da Eul", lastName: "Lee", group: "K", pic: "" },
        { name: "Dong Gun", lastName: "Lee", group: "K", pic: "" },
        { name: "Dong Yeol", lastName: "Lee", group: "K", pic: "" },
        { name: "Hoe Taek", lastName: "Lee", group: "K", pic: "" },
        { name: "Ye Dam", lastName: "Lee", group: "K", pic: "" },
        { name: "Jun Seo", lastName: "Lim", group: "K", pic: "" },
        { name: "Jung Hyun", lastName: "Mun", group: "K", pic: "" },
        { name: "Sung Min", lastName: "Oh", group: "K", pic: "" },
        { name: "Gun Wook", lastName: "Park", group: "K", pic: "" },
        { name: "Han Bin", lastName: "Park", group: "K", pic: "" },
        {
          name: "Hyun Been",
          lastName: "Park",
          group: "K",
          pic: "",
        },
        { name: "Ji Hoo", lastName: "Park", group: "K", pic: "" },
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
  background-color: pink;
  align-content: center;
  border: solid white;
  border-radius: 25px;
}
</style>
