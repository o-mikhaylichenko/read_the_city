<template>
    <button class="button">
        <span class="button__name">{{ name }}</span>
    </button>
</template>

<script>

export default {
    name: 'ButtonUi',
    components: {
    },
    props: {
        name: {
            type: String,
            default: 'Купить'
        },
    }, 
    setup() {
    }
}
</script>
<style lang="scss" scoped>
.button {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    border-radius: 7px;
    background: #3278FF;
    width: 65px;
    height: 22px;
    padding: 6px 38px;
    gap: 10px;
}
.button__name {
    color: #FFFFFF;
    text-align: center;
    font-family: Roboto;
    font-size: 20px;
    font-style: normal;
    font-weight: 500;
    line-height: 22px;
}
</style>
