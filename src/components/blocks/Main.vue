<template>
  <main class="main">
    <Card 
    :preview="require('@/assets/images/image_1book.png')"
    title="Skyrim. История создания великой игры"
    description="Франк Экстанази" 
    />
    <Card
    :preview="require('@/assets/images/image_2book.png')"
    title="Поисковое продвижение сайтов"
    description="Сергей Анисимов"
    />
    <Card 
    :preview="require('@/assets/images/image_3book.png')"
    title="Английский для дизайнеров"
    description="Татьяна Магарина"
    />
    <Card
    :preview="require('@/assets/images/image_4book.png')"
    title="Дизайн и цвет. Практикум"
    description="Шон Адамс"
    />
  </main>
</template>
  
<script>
import Card from '@/components/elements/Card'

export default {
  name: 'Main',
  components: {
    Card
  },
  props: {
  },
  setup() {
  }
}
</script>
   
<style lang="scss" scoped>
.main {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  gap: 26px;
}
</style>