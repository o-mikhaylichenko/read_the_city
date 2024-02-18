<template>
    <div class="card">
        <img class="card__preview" :src="preview" alt="">
        <div class="card__info">
            <CardInfo :title="title" :description="description" />
        </div>
        <div class="card__button">
            <ButtonUi name="Купить" />
        </div>
    </div>
</template>
  
<script>
import CardInfo from '@/components/elements/CardInfo.vue'
import ButtonUi from '@/components/ui/ButtonUi.vue'

export default {
    name: 'CardElement',
    components: {
        ButtonUi, CardInfo
    },
    props: {
        title: {
            type: String,
            default: "Name"
        },
        description: {
            type: String,
            default: "description"
        },
        preview: {
            type: String,
            default: ''
        }
    },
    setup() {

    }
}
</script>
<style lang="scss" scoped>
.card {
    display: flex;
    flex-direction: column;
    align-items: center;
    border: 1px;
    border-radius: 10px;
    background: #FFF;
    box-shadow: 1px 1px 4px 0px rgba(0, 0, 0, 0.30);
    justify-content: center;
    padding: 10px;
}
.card__info {
    display: inline-flex;
    flex-direction: column;
    align-items: center;
    gap: 14px;
    margin: 26px;
}
.card__button {
    margin-bottom: 24px;
}
</style>