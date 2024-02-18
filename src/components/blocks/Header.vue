<template>
  <header>
    <div class="header__logo">
      <div>
        <img src="@/assets/images/Logo_1.png" alt="">
      </div>
      <div class="header__tel">+7 987 654 32-10</div>
    </div>
  </header>
</template>

<script>

export default {
  name: 'HeaderPage',
  components: {
  },
  props: {
  },
  setup() {
  }
}
</script>
 
<style lang="scss" scoped>
.header__logo {
  display: flex;
  height: 60px;
  padding: 13px 70px;
  justify-content: space-between;
  align-items: center;
  gap: 10%; 
  background-color: #3278FF;
  margin-bottom: 235px;
}

.header__tel {
  color: #fff;
  font-family: Roboto;
  font-size: 22px;
  font-style: normal;
  font-weight: 600;
  line-height: normal;
}
</style>