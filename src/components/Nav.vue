<template>
  <nav>
    <router-link to="/money" class="item" active-class="selected">
      <Icon name="money"/>
      账户
    </router-link>
    <router-link to="labels" class="item" active-class="selected">
      <Icon name="label"/>
      统计
    </router-link>
    <router-link to="/statistics" class="item" active-class="selected">
      <Icon name="statistics"/>
      明细
    </router-link>
  </nav>
</template>

<script lang="ts">
// import x from '@/assets/icons/label.svg';
// import y from '@/assets/icons/money.svg';
//
// console.log(x);
// console.log(y);


export default {
  name: 'Nav.vue',
};
</script>

<style lang="scss" scoped>
nav {
  padding: 30px;
  display: flex;
  box-shadow: 0 0 3px rgba(0, 0, 0, 0.25);
  flex-direction: row;
  margin-top: auto;

  > .item {
    width: 33.33333%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    font-size: 12px;

    .icon {
      width: 26px;
      height: 26px;
    }
  }

  > .item > .selected {
    color: #63b17b;
  }
}

</style>