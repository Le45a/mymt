<template>
  <div class="m-menu">
    <dl class="nav">
      <dt>全部分类</dt>
      <dd v-for="(item,idx) in menu" :key="idx">
        <i :class="item.type" />{{ item.name }}<span class="arrow" />
      </dd>
    </dl>
    <div class="detail">
      <template>
        <h4>标题</h4>
        <span>子项</span>
      </template>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      menu: [{
        type: 'food',
        name: '美食'
      }, {
        type: 'takeout',
        name: '外卖'
      }]
    }
  }
}
</script>

<style>

</style>
