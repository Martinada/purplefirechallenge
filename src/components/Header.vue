<template>
   <div class="main-div-header">
    <div class="header-hero">
        <div class="nav-menu-items">
            <p class="logotype">antic</p>
            <img class="hamburguer-menu" src="../assets/icons/burger.svg"/>
            <div class="nav-menu-links">
                <p>Products</p>
                <p>Rooms</p>
                <p>Services</p>
                <p>Inspirations</p>
            </div>
        </div>
        <div class="main-div-body">
            <p class="text-group-label">HOME DESIGN</p>
            <p class="text-group-title">Elegance for Interiors & Exteriors</p>
            <p class="text-group-p">We provide everyone with modern, trendy, quality furniture</p>
            <a href="#design_section"><div class="arrow-scroll-down"> </div></a>
        </div>
    </div>
    <div>
        <img class="img-contact" alt="contact icon" src="../assets/icons/Contact.svg" />
      <img class="img-lamps" alt="image of a hanging lamps" src="../assets/img/lamps.jpeg" />
    </div>
  </div>
</template>

<script>
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,300;0,400;0,700;0,900;1,300;1,400;1,700;1,900&display=swap');

.main-div-header {
  display: flex;
  justify-content: space-between;
  background-color: #F3EEE8;
  @media (max-width: 680px) {
    height: 700px;
    background-image: url('../assets/img/lamps.jpeg');
    background-repeat: no-repeat;
    background-size: cover;
  }
}

.header-hero {
    padding-left: 150px;
    @media (max-width: 680px) {
        padding-left: 50px;
    }
}

.logotype {
  color: #a06056;
  font-family: 'Merriweather', serif;
  font-weight: 700;
  font-style: normal;
  font-size: 34px;
  letter-spacing: 2px;
  line-height: 25px;

  @media (max-width: 680px) {
    color: white;
    font-size: 24px;
  }
}

.hamburguer-menu {
    display: none;
    @media (max-width: 680px) {
        display: block;
        width: 30px;
        height: 30px;
  }
}
.nav-menu-items {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 50px;
  font-family: "Varta", sans-serif;
  font-optical-sizing: auto;
  font-weight: 400;
  font-style: normal;
  font-size: 18px;
  line-height: 25px;
  color: #706458;
}

.nav-menu-links {
    display: flex;
    justify-content: space-between;
    width: 300px;
    @media (max-width: 680px) {
        display: none;
    }
}

.img-contact {
    position: absolute;
    z-index: 999;
    left: 95%;
    top: 4%;
    @media (max-width: 680px) {
        display: none;
  }
}

.img-lamps {
  width: 785px;
  height: 1177px;
  position: relative;

  @media (max-width: 680px) {
    display: none;
  }
}

.main-div-body {
    margin-top: 180px;
    width: 420px;
    @media (max-width: 680px) {
        text-align: center;
        color: white;
        width: 260px;
        margin-top: 95px;
        padding-left: 70px;
        display: flex;
        flex-direction: column;
        align-items: center;
  }
}

.text-group-label {
    font-size: 14px;
    color: #a06056;
    font-family: "Varta", sans-serif;
    font-optical-sizing: auto;
    font-weight: 700;
    font-style: normal;
    @media (max-width: 680px) {
        text-align: center;
        color: white;
  }
}

.text-group-title {
    color: #a06056;
    font-family: 'Merriweather', serif;
    font-weight: 300;
    font-style: normal;
    font-size: 50px;
    margin-top: 20px;
    line-height: 70px;
    letter-spacing: -0.4px;
    @media (max-width: 680px) {
        text-align: center;
        color: white;
        font-size: 25px;
        line-height: 40px;
  }
}

.text-group-p {
    color: #706458E5;
    font-family: "Varta", sans-serif;
    font-optical-sizing: auto;
    font-weight: 300;
    font-style: normal;
    font-size: 22px;
    line-height: 30.8px;
    margin-top: 15px;
    @media (max-width: 680px) {
        text-align: center;
        color: white;
        font-size: 14px;
        line-height: 22px;
  }
}

.arrow-scroll-down {
    width: 100px;
    height: 100px;
    background: url('../assets/icons/arrow-scroll.svg') no-repeat;
    margin-top: 60px;
}
.arrow-scroll-down:hover {
    background: url('../assets/icons/arrow-scroll-hover.svg') no-repeat;
}
</style>
