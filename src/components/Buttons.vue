<template>
    <button>
        <i>
            <slot name="icon"></slot>
        </i>
        <p class="button-style">
        <slot name="title"></slot>
      </p>
    </button>
</template>

<style scoped>
.primary-grey {
    font-family: Karla;
    font-weight: 700;
    line-height: 25px;
    letter-spacing: 0.3px;
    text-align: center;
    background-color: #534B42;
    padding: 8px 30px;
    color: white;
    font-size: 17px;
}
.primary {
    font-family: Inter;
    padding: 10px 20px;
    border: none;
    font-size: 18px;
    font-weight: 500;
    line-height: 21.78px;
    text-align: left;
    color: white;
    background-color: #E73C17;
}
.primary:hover {
    background-color: #C22900;
}

.secondary {
    color: #E73C17;
    border: #E73C17;
}
.secondary:hover {
    background-color: #F3F3F3;
}

.suscribed {
    background-color: #191919;
}
</style>