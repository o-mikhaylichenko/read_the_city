<template>
  <div class="">
    <Header></Header>
    <Main></Main>
  </div>
</template>

<script>
import Header from '@/components/blocks/Header'
import Main from '@/components/blocks/Main'

export default {
  name: 'MainPage',
  components: {
    Header,
    Main
  },
  props: {
  },
  setup () {
  }
}
</script>

<style lang="scss" scoped></style>
