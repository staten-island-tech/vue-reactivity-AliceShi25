<template>
  <div class="main">
    <h1>Invest in Stars</h1>
    <div class="parent">
      <TheCards
        v-for="star in stars"
        :key="star.name"
        :name="star.name"
        :lastname="star.lastName"
        :image="star.img"
        :group="star.group"
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
          name: "Anthonny",
          lastName: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/3e7fd9ae29da307bbb9010b72670fdec_m.webp",
        },
        {
          name: "Brian",
          lastName: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/3ffa288aee37322ca336d3e7b889f85a_m.webp",
        },
        {
          name: "Jin Xin",
          lastName: "Cai",
          group: "G",
          img: "https://img.kpopjuice.com/member/03e2d4f1067535ecbe0b48c0c08e466f_m.webp",
        },
        {
          name: "Do Ha",
          lastName: "Bak",
          group: "K",
          img: "https://img.kpopjuice.com/member/5f89c00d842a3e03901f4b3eccd7873d_m.webp",
        },
        {
          name: "Woong Ki",
          lastName: "Cha",
          group: "K",
          img: "https://img.kpopjuice.com/member/75945aca822638f1b3b98a0b93155fba_m.webp",
        },
        {
          name: "Jian Yu",
          lastName: "Chen",
          group: "G",
          img: "https://img.kpopjuice.com/member/746780c089e938e482383df6766856d3_m.webp",
        },
        {
          name: "Kuan Jui",
          lastName: "Chen",
          group: "G",
          img: "https://img.kpopjuice.com/member/6d70054717143dc88e291cf36ce720e6_m.webp",
        },
        {
          name: "Liang",
          lastName: "Chen",
          group: "G",
          img: "https://img.kpopjuice.com/member/50f2877586bd36d4bda39f7764456457_m.webp",
        },
        {
          name: "Ren You",
          lastName: "Chen",
          group: "G",
          img: "https://img.kpopjuice.com/member/f316b09cd06931b1a043e31123c64f43_m.webp",
        },
        {
          name: "Ji Ho",
          lastName: "Choi",
          group: "K",
          img: "https://img.kpopjuice.com/member/a427e56b805b3292878a4d55de4e2f8c_m.webp",
        },
        {
          name: "Seung Hun",
          lastName: "Choi",
          group: "K",
          img: "https://img.kpopjuice.com/member/684245793f3b3973bc3dfeb730923760_m.webp",
        },
        {
          name: "Woo Jin",
          lastName: "Choi",
          group: "K",
          img: "https://img.kpopjuice.com/member/280c80bfe8083d6bb9c206476569972a_m.webp",
        },
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
.parent {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  flex-direction: row;
  padding: 2.5rem;
  text-align: center;
}
.main {
  text-align: center;
}
</style>
