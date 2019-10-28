<template>
  <div class="home">
    <searchBar
      disabled
      @onClick="onSearchBarkClick"
    />
    <HomeCard/>
    <HomeBanner
      img="http://www.youbaobao.xyz/book/res/bg.jpg"
      title="mpvue2.0实战多端小程序课程上线啦"
      subTitle="立即体验"
      @onClick="onBannerClick"
    />
  </div>
</template>

<script>
  import SearchBar from '../../components/home/SearchBar'
  import HomeCard from '../../components/home/HomeCard'
  import HomeBanner from '../../components/home/HomeBanner'
  export default {
    components: {
      HomeBanner,
      HomeCard,
      SearchBar
    },
    methods: {
      // 搜索跳转页
      onSearchBarkClick() {
      }
    }
  }
</script>

<style lang="stylus" scoped>
  .book-home {
    margin-top: 23px;
  }
</style>
