<template>
  <div class="main">
    <h2>Invest in Stars</h2>
    <div class="cart">
      <TheCart />
    </div>
    <div class="bros">
      <TheCards
        v-for="star in stars"
        :key="star.name"
        :name="star.name"
        :lastname="star.lastname"
        :image="star.img"
        :group="star.group"
      />
    </div>
  </div>
</template>

<script>
import TheCards from "../components/TheCards.vue";
import TheCart from "../components/TheCart.vue";

export default {
  name: "ProductsList",
  components: { TheCards, TheCart },
  data() {
    return {
      selected: "",
      stars: [
        {
          name: "Anthonny",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/3e7fd9ae29da307bbb9010b72670fdec_m.webp",
        },
        {
          name: "Do Ha",
          lastname: "Bak",
          group: "K",
          img: "https://img.kpopjuice.com/member/5f89c00d842a3e03901f4b3eccd7873d_m.webp",
        },
        {
          name: "Brian",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/3ffa288aee37322ca336d3e7b889f85a_m.webp",
        },
        {
          name: "Jin Xin",
          lastname: "Cai",
          group: "G",
          img: "https://img.kpopjuice.com/member/03e2d4f1067535ecbe0b48c0c08e466f_m.webp",
        },
        {
          name: "Woong Ki",
          lastname: "Cha",
          group: "K",
          img: "https://img.kpopjuice.com/member/75945aca822638f1b3b98a0b93155fba_m.webp",
        },
        {
          name: "Jian Yu",
          lastname: "Chen",
          group: "G",
          img: "https://img.kpopjuice.com/member/746780c089e938e482383df6766856d3_m.webp",
        },
        {
          name: "Kuan Jui",
          lastname: "Chen",
          group: "G",
          img: "https://img.kpopjuice.com/member/6d70054717143dc88e291cf36ce720e6_m.webp",
        },
        {
          name: "Liang",
          lastname: "Chen",
          group: "G",
          img: "https://img.kpopjuice.com/member/50f2877586bd36d4bda39f7764456457_m.webp",
        },
        {
          name: "Ren You",
          lastname: "Chen",
          group: "G",
          img: "https://img.kpopjuice.com/member/f316b09cd06931b1a043e31123c64f43_m.webp",
        },
        {
          name: "Ji Ho",
          lastname: "Choi",
          group: "K",
          img: "https://img.kpopjuice.com/member/a427e56b805b3292878a4d55de4e2f8c_m.webp",
        },
        {
          name: "Seung Hun",
          lastname: "Choi",
          group: "K",
          img: "https://img.kpopjuice.com/member/684245793f3b3973bc3dfeb730923760_m.webp",
        },
        {
          name: "Woo Jin",
          lastname: "Choi",
          group: "K",
          img: "https://img.kpopjuice.com/member/280c80bfe8083d6bb9c206476569972a_m.webp",
        },
        {
          name: "Cong",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/0e8dc96e86d33326abf30819df301a56_m.webp",
        },
        {
          name: "Crayon",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/4afa622271f2382cb3604a9ae914b7a9_m.webp",
        },
        {
          name: "Hong Hai",
          lastname: "Dang",
          group: "G",
          img: "https://img.kpopjuice.com/member/a626fbfc19443a7d9b3c6ef6c6a860a4_m.webp",
        },
        {
          name: "Dong Dong",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/7189c9d3a14b38c4adc89a2bda24bb8a_m.webp",
        },
        {
          name: "Jun Lan",
          lastname: "Feng",
          group: "G",
          img: "https://img.kpopjuice.com/member/a336ad8598483095a02472091c227b7c_m.webp",
        },
        {
          name: "Seo Bin",
          lastname: "Han",
          group: "K",
          img: "https://img.kpopjuice.com/member/f8a660cf9db239e9a40d22f63f484c44_m.webp",
        },
        {
          name: "Yu Jin",
          lastname: "Han",
          group: "K",
          img: "https://img.kpopjuice.com/member/583c3afd60db3feeb1a6a0f214ef9dfa_m.webp",
        },
        {
          name: "Yu Seop",
          lastname: "Han",
          group: "K",
          img: "https://img.kpopjuice.com/member/2635e71a44e13af6bbc9ac2902021447_m.webp",
        },
        {
          name: "Haru",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/6aebb0bbd8d63ec3bd4bed453ea1a0ff_m.webp",
        },
        {
          name: "Haruto",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/395883cc7f88339a919cf173069e829c_m.webp",
        },
        {
          name: "Keon Hee",
          lastname: "Hong",
          group: "K",
          img: "https://img.kpopjuice.com/member/d66d706045ba319ca7a20858878987e0_m.webp",
        },
        {
          name: "Hyo",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/44452fc9f0e13f3ba45252a5454e5cb8_m.webp",
        },
        {
          name: "Ichika",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/ccdbd5f969ce3400bb3ac823a61bfd8e_m.webp",
        },
        {
          name: "Hiroto",
          lastname: "Ikumi",
          group: "G",
          img: "https://img.kpopjuice.com/member/2b255eaff58639cfab603767836c554d_m.webp",
        },
        {
          name: "Itsuki",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/2669a04a075939d49a7c246b8392469a_m.webp",
        },
        {
          name: "Ji Ho",
          lastname: "Jang",
          group: "K",
          img: "https://img.kpopjuice.com/member/2b924622c7b93ae38bb9fddcfc548251_m.webp",
        },
        {
          name: "Min Seo",
          lastname: "Jang",
          group: "K",
          img: "https://img.kpopjuice.com/member/cd494fcfaaa33273a70b287305df941e_m.webp",
        },
        {
          name: "Yeo Jun",
          lastname: "Jang",
          group: "K",
          img: "https://img.kpopjuice.com/member/34a2bf7b24c23fab964c3972f880f903_m.webp",
        },
        {
          name: "Jay",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/222129faf0b33582ac43a5338e901d4e_m.webp",
        },
        {
          name: "I Chan",
          lastname: "Jeong",
          group: "K",
          img: "https://img.kpopjuice.com/member/e3d2620fffc430e6b9d3516f1cb8f7c2_m.webp",
        },
        {
          name: "Ho Young",
          lastname: "Jeong",
          group: "K",
          img: "https://img.kpopjuice.com/member/c9a48350c9413af8b91763240dca1090_m.webp",
        },
        {
          name: "Woo Seok",
          lastname: "Jeon",
          group: "K",
          img: "https://img.kpopjuice.com/member/ed90b2d7e5ac3e2aae6427b1cb735204_m.webp",
        },
        {
          name: "Yun Seo",
          lastname: "Ji",
          group: "K",
          img: "https://img.kpopjuice.com/member/34e2f3b82e8931e29eb1c8881130d331_m.webp",
        },
        {
          name: "Ho Jin",
          lastname: "Jung",
          group: "K",
          img: "https://img.kpopjuice.com/member/6b2a65eae8ca30dfa88ba119b08ac6b9_m.webp",
        },
        {
          name: "Hwan Rok",
          lastname: "Jun",
          group: "K",
          img: "https://img.kpopjuice.com/member/180158042c183b4e9e1aa6426312e367_m.webp",
        },
        {
          name: "Min Gyu",
          lastname: "Jung",
          group: "K",
          img: "https://img.kpopjuice.com/member/cfbfbe3cb3c0370084304d43ee5819a8_m.webp",
        },
        {
          name: "Se Yun",
          lastname: "Jung",
          group: "K",
          img: "https://img.kpopjuice.com/member/0d3e30adef9537c4a196c737fbe77ebe_m.webp",
        },
        {
          name: "Kei",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/772ac7de0b5c3fe6adc011d95d8c821c_m.webp",
        },
        {
          name: "Keita",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/75e4bb4c02e737f28e8117602c086508_m.webp",
        },
        {
          name: "Gyu Vin",
          lastname: "Kim",
          group: "K",
          img: "https://img.kpopjuice.com/member/a44f6eec008039b49764eb285759cca2_m.webp",
        },
        {
          name: "Ji Woong",
          lastname: "Kim",
          group: "K",
          img: "https://img.kpopjuice.com/member/c1633cbc9bdf37a78b986b2ea9639dcf_m.webp",
        },
        {
          name: "Min Hyuk",
          lastname: "Kim",
          group: "K",
          img: "https://img.kpopjuice.com/member/7221f74e46763450a0ddbe27c995ab28_m.webp",
        },
        {
          name: "Min Seoung",
          lastname: "Kim",
          group: "K",
          img: "https://img.kpopjuice.com/member/666b3ec299333709ad2d8996daffb7c9_m.webp",
        },
        {
          name: "Tae Rae",
          lastname: "Kim",
          group: "K",
          img: "https://img.kpopjuice.com/member/d916877e7fd93b2d96cf66e5a100c46d_m.webp",
        },
        {
          name: "Krystian",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/4efa5674cf103bd0ab83d6f87ef642c9_m.webp",
        },
        {
          name: "Jun Hyeon",
          lastname: "Kum",
          group: "K",
          img: "https://img.kpopjuice.com/member/f937b36216f13e6b88ea9411317a2e04_m.webp",
        },
        {
          name: "Da Eul",
          lastname: "Lee",
          group: "K",
          img: "https://img.kpopjuice.com/member/ce1cd43502c3368cbb36b903f2cb2187_m.webp",
        },
        {
          name: "Dong Gun",
          lastname: "Lee",
          group: "K",
          img: "https://img.kpopjuice.com/member/29a283992b8030d3a8e82a89efe44cd3_m.webp",
        },
        {
          name: "Dong Yeol",
          lastname: "Lee",
          group: "K",
          img: "https://img.kpopjuice.com/member/a80cc4825f8c36b78536328bd10f5b37_m.webp",
        },
        {
          name: "Hoe Taek",
          lastname: "Lee",
          group: "K",
          img: "https://img.kpopjuice.com/member/a766fc13b7953eddb8c1dc93618e5700_m.webp",
        },
        {
          name: "Hwan",
          lastname: "Hee",
          group: "K",
          img: "https://img.kpopjuice.com/member/8b329282388b3ddf92ab851beb4d37ad_m.webp",
        },
        {
          name: "Jeong Hyeon",
          lastname: "Lee",
          group: "K",
          img: "https://img.kpopjuice.com/member/970996ab563239489a0f2ccdbe4ed9e0_m.webp",
        },
        {
          name: "Seung Hwan",
          lastname: "Lee",
          group: "K",
          img: "https://img.kpopjuice.com/member/2c0adf6c25533e1f9a17cf4a3c278bff_m.webp",
        },
        {
          name: "Ye Dam",
          lastname: "Lee",
          group: "K",
          img: "https://img.kpopjuice.com/member/6e1f9a3291543af3beb5ff9c4c5840b5_m.webp",
        },
        {
          name: "Jun Seo",
          lastname: "Lim",
          group: "K",
          img: "https://img.kpopjuice.com/member/4c49cd12806631699c2333685318160a_m.webp",
        },
        {
          name: "Shi Yuan",
          lastname: "Lin",
          group: "G",
          img: "https://img.kpopjuice.com/member/e8f7ce5353ba3aaca8fb4b04faa1e17f_m.webp",
        },
        {
          name: "Jin Xiang",
          lastname: "Ma",
          group: "G",
          img: "https://img.kpopjuice.com/member/616ef57120783f45bc57b2641de84957_m.webp",
        },
        {
          name: "Min",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/75e87941e9583c888c8419affffda4b3_m.webp",
        },
        {
          name: "Jung Hyun",
          lastname: "Mun",
          group: "K",
          img: "https://img.kpopjuice.com/member/b6bad9b258d7380ea2cb1865d6205bce_m.webp",
        },
        {
          name: "Kamden",
          lastname: "Na",
          group: "G",
          img: "https://img.kpopjuice.com/member/e62d98f16c393626966b7440d69c0412_m.webp",
        },
        {
          name: "Nice",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/0891f249ff913ee5bf3ee1e9cd8b36c0_m.webp",
        },
        {
          name: "Sung Min",
          lastname: "Oh",
          group: "K",
          img: "https://img.kpopjuice.com/member/53d1acc6e3c03190b037aee07538d3de_m.webp",
        },
        {
          name: "Ollie",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/848b2a3af28c3b0580deb58485ccf350_m.webp",
        },
        {
          name: "Osuke",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/1be5a1157dd53aa69e841d313c1ecf4d_m.webp",
        },
        {
          name: "Ouju",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/162a9cb590563d4bb7d88ee286b03ed3_m.webp",
        },
        {
          name: "Gun Wook",
          lastname: "Park",
          group: "K",
          img: "https://img.kpopjuice.com/member/cd576ae6e0c13c979a4de7a1c547fddb_m.webp",
        },
        {
          name: "Gwan Young",
          lastname: "Park",
          group: "K",
          img: "https://img.kpopjuice.com/member/dc2c458171673bc2a7f5cc3439870576_m.webp",
        },
        {
          name: "Han Bin",
          lastname: "Park",
          group: "K",
          img: "https://img.kpopjuice.com/member/4f84db4f5f7e38beabcd9c3e81fb81a1_m.webp",
        },
        {
          name: "Hyun Been",
          lastname: "Park",
          group: "K",
          img: "https://img.kpopjuice.com/member/c5f2f394332e39938d0182985ebb997a_m.webp",
        },
        {
          name: "Ji Hoo",
          lastname: "Park",
          group: "K",
          img: "https://img.kpopjuice.com/member/c78299a5f0623e178bdd1160e5165152_m.webp",
        },
        {
          name: "Min Seok",
          lastname: "Park",
          group: "K",
          img: "https://img.kpopjuice.com/member/4354cbbf47f63ec7b9a4613304d89203_m.webp",
        },
        {
          name: "Sheng Yang",
          lastname: "Qiu",
          group: "G",
          img: "https://img.kpopjuice.com/member/4e3ced7cae7f37009f429e4af5fa16f6_m.webp",
        },
        {
          name: "Ricky",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/72222c51f08a3e54974206f92806f785_m.webp",
        },
        {
          name: "Riku",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/2452e9854ca4391bbaa20d80beda5412_m.webp",
        },
        {
          name: "Matthew",
          lastname: "Seok",
          group: "G",
          img: "https://img.kpopjuice.com/member/c75f0ed93a153e5ba42ed93537fd5b69_m.webp",
        },
        {
          name: "Won",
          lastname: "Seo",
          group: "K",
          img: "https://img.kpopjuice.com/member/061a6b46d9cb3e638f72a27477b4aa47_m.webp",
        },
        {
          name: "Han Bin",
          lastname: "Sung",
          group: "K",
          img: "https://img.kpopjuice.com/member/82546f349cf438c2b339e5e3d92d3390_m.webp",
        },
        {
          name: "Takuto",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/ba13372236cb37cabeaf4331c5084b56_m.webp",
        },
        {
          name: "Toui",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/629187e181f23282a871465f4b23e358_m.webp",
        },
        {
          name: "Yan Hong",
          lastname: "Wang",
          group: "G",
          img: "https://img.kpopjuice.com/member/bfbc7cdddcb631899a70b89096798e93_m.webp",
        },
        {
          name: "Zi Hao",
          lastname: "Wang",
          group: "G",
          img: "https://img.kpopjuice.com/member/38ac5eac9d6d3dd7a973b2ad46ebb20e_m.webp",
        },
        {
          name: "Ye Chen",
          lastname: "Wen",
          group: "G",
          img: "https://img.kpopjuice.com/member/d02ab8cfe76d38549083e00cb4f0ffe3_m.webp",
        },
        {
          name: "Winnie",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/3fc7487e3fba3c1fbfb68f54d82d6aa6_m.webp",
        },
        {
          name: "Wumuti",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/dee98415a6b53500b5207dacf0e0318c_m.webp",
        },
        {
          name: "Hao",
          lastname: "Xuan",
          group: "G",
          img: "https://img.kpopjuice.com/member/f79a9c501f6a3189a2657a00c7067014_m.webp",
        },
        {
          name: "Jun",
          lastname: "Yang",
          group: "G",
          img: "https://img.kpopjuice.com/member/385b83be91193fbe8fb4133dc5e087ee_m.webp",
        },
        {
          name: "Joong Woo",
          lastname: "Yoo",
          group: "K",
          img: "https://img.kpopjuice.com/member/8563fa78d74b3f0e8e2345beb2e12f5d_m.webp",
        },
        {
          name: "Seung Eon",
          lastname: "Yoo",
          group: "K",
          img: "https://img.kpopjuice.com/member/0bb4a6e7054a35ed9329d8ef98f1d7d8_m.webp",
        },
        {
          name: "Yuki",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/08068668e8313769a2e94ee8177e748d_m.webp",
        },
        {
          name: "Yutaka",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/be5b3d51661834519cf023031c07daf8_m.webp",
        },
        {
          name: "Yuto",
          lastname: "",
          group: "G",
          img: "https://img.kpopjuice.com/member/73aae23ca329343c927e7bf0d70af917_m.webp",
        },
        {
          name: "Hao",
          lastname: "Zhang",
          group: "G",
          img: "https://img.kpopjuice.com/member/13afdf8ff57539779f2eadb518175104_m.webp",
        },
        {
          name: "Shuai Bo",
          lastname: "Zhang",
          group: "G",
          img: "https://img.kpopjuice.com/member/6fad94a98c3d3a5f83f6d5f7e4cc0d22_m.webp",
        },
      ],
    };
  },
  methods: {},
};
</script>

<style scoped>
.cart {
  display: flex;
  flex-direction: row;
}
.bros {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  flex-direction: row;
  padding: 2.5rem;
  text-align: center;
  background-color: #1b1545;
}
.main {
  text-align: center;
}
</style>
