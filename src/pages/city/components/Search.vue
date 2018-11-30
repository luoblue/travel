<template>
    <div class="search">
      <input class="search-input" type="text" placeholder="输入城市名或拼音">
    </div>
</template>

<script>
export default {
  name: 'CitySearch'
}
</script>

<style scoped lang="stylus">
  @import "~style/varibles.styl";
  .search{
    height: .72rem;
    background: $bgColor;
    padding: 0 .1rem;
    .search-input{
      -webkit-box-sizing: border-box
      -moz-box-sizing: border-box
      box-sizing: border-box
      width: 100%;
      height: .62rem;
      padding: 0 .1rem;
      line-height: .62rem;
      text-align: center;
      -webkit-border-radius: .06rem;
      -moz-border-radius: .06rem;
      border-radius: .06rem;
      color: #666;
    }
  }
</style>
