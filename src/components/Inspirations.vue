<template>
    <img class="slider-imgs" src="../assets/img/Slides.png" alt="furniture images" />
    <div class="slider-inspirations">
        <p class="slider-title">Inspirations</p>
        <p class="slider-descp">Our experts are keen to stay on top of trends in order to offer you new inspirations
            for your interior and exterior every day. Remember that to inspire you we have to inspire ourselves and we want to share that with you.</p>
        <div class="pagination-div">
            <img class="arrow-left" />
            <img class="arrow-right" />
            <p class="slider-pagination">01 / 05</p>
        </div>
    </div>
</template>

<style>

.slider-imgs {
    @media (max-width: 680px) {
        width: 400px;
    }
}

.slider-inspirations {
    display: flex;
    justify-content: space-between;
    padding: 50px 150px;
    @media (max-width: 680px) {
        display: block;
        padding-left: 50px;
    }
}
.slider-title {
    font-family: Merriweather;
    font-size: 45px;
    font-weight: 300;
    line-height: 40px;
    letter-spacing: -0.3px;
    text-align: left;
    color: #534B42;
    @media (max-width: 680px) {
     font-size: 30px;   
    }
}
.slider-descp {
    font-family: Varta;
    font-size: 18px;
    font-weight: 400;
    line-height: 25px;
    text-align: left;
    color: #706458;
    width: 359px;
    @media (max-width: 680px) {
        margin-top: 15px;
        width: 325px;
    }
}

.pagination-div {
    @media (max-width: 680px) {
        display: none;
    }
}
.arrow-left {
    width: 80px;
    height: 80px;
    background: url('../assets/icons/arrow-left.svg') no-repeat;
}
.arrow-left:hover {
    background: url('../assets/icons/arrow-left-hover.svg') no-repeat;
}
.arrow-right {
    width: 80px;
    height: 80px;
    border: none;
    background: url('../assets/icons/arrow-right-2.svg') no-repeat;
}
.arrow-right:hover {
    background: url('../assets/icons/arrow-right-hover.svg') no-repeat;
}

.slider-pagination {
    font-family: Varta;
    font-size: 18px;
    font-weight: 400;
    line-height: 25px;
    text-align: left;
    color: rgba(112, 100, 88, 0.9);
}
</style>