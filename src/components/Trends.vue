<template>
    <div class="trends-newsletter-div">
        <div>
            <p class="trends-title">Be aware of the latest trends</p>
            <p class="trends-subtitle">Stay informed of new trends, but also of our various offers.</p>
            <p class="design-sec-link">Learn more <img src="../assets/icons/Right.svg" /></p>
        </div>
        <div>
            <input class="email-input" placeholder="email@address.com"></input>
            <Buttons class="primary-grey" >
                <template #title>Subscribe</template>
            </Buttons>
        </div>
    </div>
</template>

<script setup>
import Buttons from './Buttons.vue'
</script>

<style>
.trends-newsletter-div {
    display: flex;
    justify-content: space-between;
    padding: 50px 150px;

    @media (max-width: 680px) {
        display: block;
        padding-left: 50px;
        padding-top: 20px;
    }
}

.trends-title {
    font-family: Merriweather;
    font-size: 35px;
    font-weight: 400;
    line-height: 40px;
    letter-spacing: -0.3px;
    text-align: left;
    color: #121212;

    @media (max-width: 680px) {
        text-align: unset;
    }
}

.trends-subtitle {
    font-family: Varta;
    font-size: 18px;
    font-weight: 400;
    line-height: 25px;
    text-align: left;
    color: #706458E5;
    margin-top: 15px;

}

.design-sec-link {
    margin-top: 30px;
    font-family: "Karla", sans-serif;
    font-size: 17px;
    font-weight: 700;
    line-height: 25px;
    letter-spacing: 0.3px;
    color: #a06056;
    text-align: left;
    display: flex;
    align-items: center;
}

.email-input {
    width: 296px;
    height: 50px;
    border-radius: 1px;
    border: none;
    background-color: #F3EEE84D;;
    margin-right: 12px;

    @media (max-width: 680px) {
        margin-top: 30px;
        margin-bottom: 15px;
    }
}
.email-input::placeholder {
    font-family: Varta;
    font-weight: 400;
    line-height: 25px;
    text-align: left;
    padding-left: 12px;
    color: #706458E5;
    font-size: 18px;
}
</style>