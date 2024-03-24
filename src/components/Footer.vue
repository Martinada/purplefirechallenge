<template>
  <div class="main-footer-div">
    <div class="columns-main-div">
      <p class="logotype-footer">antic</p>
      <div class="columns-footer">
        <div class="column-div" v-for="item in columns" :key="item.title">
          <p class="columns-title">{{ item.title }}</p>
          <ul>
            <li class="columns-items" v-for="elem in item.elements">
              {{ elem }}
            </li>
          </ul>
        </div>
      </div>
      <div>
        <p class="columns-title">We respect our planet</p>
        <img class="img-furniture" src="../assets/img/furniture.png" />
        <p class="desc-furniture">
          We’re taking positive steps to reduce our impact on the planet. For us, that means
          retailing responsibly.
        </p>
        <p class="design-sec-link">Learn more <img src="../assets/icons/Right.svg" /></p>
      </div>
    </div>
    <div class="copyright-div">
      <div class="socials-div">
        <img src="../assets/icons/Facebook.png" />
        <img src="../assets/icons/Twitter.png" />
        <img src="../assets/icons/Linkedin.png" />
        <img src="../assets/icons/Instagram.png" />
      </div>
      <div class="legals">
        <p class="agence">© 2021 Agence Dnd</p>
        <p>Privacy policy</p>
        <p>Term of service</p>
        <p>Language</p>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  setup() {
    const columns = [
      {
        title: 'Products',
        elements: ['Furniture', 'Decoration', 'Storage', 'Baby and child', 'Connected home']
      },
      {
        title: 'Rooms',
        elements: [
          'Living room',
          'Dining room',
          'Cooked',
          'Bedroom',
          'Bathroom',
          'Office',
          'Laundry',
          'Garage'
        ]
      },
      {
        title: 'Services',
        elements: ['Click and collect', 'Conception', 'Installation', 'Advices', 'Gift card']
      },
      {
        title: 'About',
        elements: ['Our story', 'Our stores', 'Our partners']
      }
    ]

    return { columns }
  }
}
</script>

<style>
.main-footer-div {
  padding: 50px 150px;
  background-color: #f3eee8;
  gap: 48px;
  display: grid;
  @media (max-width: 680px) {
    display: block;
    padding-left: 50px;
  }
}
.columns-main-div {
  display: flex;
  justify-content: space-between;
  @media (max-width: 680px) {
    display: block;
  }
}
.logotype-footer {
  color: #534b42;
  font-family: 'Merriweather', serif;
  font-weight: 700;
  font-style: normal;
  font-size: 34px;
  letter-spacing: 2px;
  line-height: 25px;
  @media (max-width: 680px) {
    text-align: center;
  }
}
.column-div {
  @media (max-width: 680px) {
    margin-bottom: 40px;
  }
}
.columns-footer {
  width: 650px;
  display: flex;
  justify-content: space-between;
  @media (max-width: 680px) {
    display: block;
    margin-top: 25px;
  }
}
.columns-title {
  font-family: Varta;
  font-size: 25px;
  font-weight: 600;
  line-height: 30px;
  letter-spacing: -0.2px;
  text-align: left;
  color: #534b42;
}
.columns-items {
  margin-top: 15px;
  font-family: Varta;
  font-size: 18px;
  font-weight: 400;
  line-height: 25px;
  text-align: left;
  color: #706458;
  @media (max-width: 680px) {
    line-height: 15px;
  }
}
ul {
  list-style-type: none;
  padding-left: unset;
}
.img-furniture {
  margin-top: 15px;
}

.socials-div {
  display: flex;
  width: 1140px;
  justify-content: center;
  gap: 24px;
  @media (max-width: 680px) {
    display: block;
  }
}

.desc-furniture {
  width: 235px;
  height: 100px;
  font-family: Varta;
  font-size: 16px;
  font-weight: 400;
  line-height: 25px;
  text-align: left;
  color: #706458;
}
.copyright-div {
  width: 1140px;
  gap: 20px;
}

.legals {
  display: flex;
  justify-content: space-between;
  width: 1140px;
  font-family: Varta;
  font-size: 18px;
  font-weight: 400;
  line-height: 25px;
  text-align: left;
  color: #706458b2;
  opacity: 70%;
  @media (max-width: 680px) {
    display: block;
  }
}

.agence {
  width: 790px;
  height: 25px;
}
</style>
