<template>
    <div class="item">
      <p class="item-title">
        <slot name="title"></slot>
      </p>
      <slot class="item-text" name="text"></slot>
    </div>
</template>

<script>
</script>

<style scoped>
.item {
    width: 300px;
    padding-top: 25px;
}
.item-title {
    font-size: 25px;
    color: #A06056;
    font-family: Varta;
    font-weight: 600;
    line-height: 30px;
    letter-spacing: -0.2px;
    text-align: left;
}

.item-text {
    font-family: Varta;
    font-size: 18px;
    font-weight: 400;
    line-height: 25px;
    text-align: left;
    color: #706458E5;
}
</style>