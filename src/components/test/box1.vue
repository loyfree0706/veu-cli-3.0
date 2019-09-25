<template lang="pug">
    div
      div.box1
      div
        img(src="/public/images/home.jpg")
        
        //- 可以讀取
        //- img(src="../../../public/images/home.jpg")
        //- 可以讀取
        //- img(src="../../assets/images/home.jpg")

        //- img(:src='url2')
        //- img(:src='url3')
        //- img(:src='url4')
        //- img(:src='url5')
        //- img(:src='url6')
        //- 編譯錯誤
        //- img(:src='url7')
        //- 可以讀取
        //- img(:src='url8')
        //- 可以讀取
        //- img(:src='url9')

</template>

<script>
import url1 from '../../assets/images/home.jpg'

export default {
  name: 'box',
  data() {
    return {
      publicPath: process.env.BASE_URL,
      //若將資源放置在assets
      url1: url1, //可讀取
      url2: "../assets/home.png", //無法讀取
      url3: "@assets/imagers/home.jpg", //無法讀取
      //若將資源放置在public
      url4: "../../../public/images/home.jpg", //無法讀取
      url5: "/public/images/home.jpg", //無法讀取
      url6: "`${publicPath}/images/home.jpg`", //無法讀取
      // url7: require('@assets/images/home.jpg') //編譯錯誤
      url8: require('../../../public/images/home.jpg'), //可讀取
      url9: require('../../assets/images/home.jpg'), //可讀取
    }
  }
};
</script>

<style lang="sass">
    .box1
        height: 500px
        width: 500px
        background: black
        display: inline-block
</style>