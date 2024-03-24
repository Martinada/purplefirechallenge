<template>
    <div id="design_section" class="main-div-design">
        <div>
            <p class="design-sec-title">We stay by your side to design your projects</p>
            <p class="design-sec-link">Find out more <img src="../assets/icons/Right.svg" /></p>
        </div>
        <div>
            <div class="items">
                <SideToDesignSections>
                    <template #title>Our devices</template>
                    <template #text>What if you took advantage of this rather special period to rethink your interior? You spend more time at home so you might as well feel good there.</template>
                </SideToDesignSections>
                <SideToDesignSections>
                    <template #title>Click and Collect</template>
                    <template #text>Adapted and contactless. Free from € 200 of purchases in stores offering the service.</template>
                </SideToDesignSections>
            </div>
            <div class="items">
                <SideToDesignSections>
                    <template #title>Conception Service</template>
                    <template #text>Personalized service with an expert advisor for your interior and exterior decoration or layout projects. </template>
                </SideToDesignSections>
                <SideToDesignSections>
                    <template #title>Installation Service</template>
                    <template #text>Our furniture packaged in flat packs are designed for easy assembly. But you can call on our partner.</template>
                </SideToDesignSections>
            </div>
        </div>
    </div>
</template>

<script setup>
    import SideToDesignSections from './SideToDesignSections.vue'
</script>

<style>
.main-div-design {
    background-color: #F3EEE8;
    padding: 50px 150px;
    display: flex;
    justify-content: space-between;
    @media (max-width: 680px) {
        padding-left: 50px;
        display: block;
    }
}

.items {
    display: flex;
    @media (max-width: 680px) {
        display: block;
    }
}
.design-sec-title {
    font-family: Merriweather;
    font-size: 55px;
    font-weight: 400;
    line-height: 60px;
    letter-spacing: -0.6px;
    text-align: left;
    width: 458px;
    color: #706458;
    @media (max-width: 680px) {
        font-size: 30px; 
        line-height: 40px; 
        text-align: unset;
        width: 240px;
    }

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
</style>