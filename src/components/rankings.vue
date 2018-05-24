<template>
    <div class="container">
        <ul>
            <li>
                <img src="//gw.alicdn.com/tps/i1/T19LocFghXXXXsGF3s-640-640.png" alt="">
                <p>虾米音乐榜</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="//gw.alicdn.com/tps/i1/T1qMgSFlxkXXXsGF3s-640-640.png" alt="">
                <p>虾米原创榜</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="//img.alicdn.com/tps/TB1RTkfNVXXXXXdXFXXXXXXXXXX-290-290.png" alt="">
                <p>中文排行榜</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="//img.alicdn.com/tps/TB1GMQvNVXXXXbwXXXXXXXXXXXX-290-290.png" alt="">
                <p>香港劲歌榜</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="//img.alicdn.com/tps/TB1EqgvNVXXXXbPXXXXXXXXXXXX-290-290.png" alt="">
                <p>Billboard 榜</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="//img.alicdn.com/tps/TB17O3cNVXXXXa0XFXXXXXXXXXX-290-290.png" alt="">
                <p>酷狗单曲榜</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="//img.alicdn.com/tps/TB1K.ErNVXXXXXcXpXXXXXXXXXX-290-290.png" alt="">
                <p>M-net 周榜</p>
                <div class="next"></div>
            </li>
        </ul>
    </div>
</template>
<script>
import axios from "axios";
export default {
  name: "rankings",
  data:function(){
      return{
          item:[]
      };
  },
  mounted:function(){
      console.log('-----------');
//       axios.get("https://c.y.qq.com/v8/fcg-bin/fcg_v8_toplist_cp.fcg?g_tk=5381&uin=0&format=json&inCharset=utf-8&outCharset=utf-8&notice=0&platform=h5&needNewCode=1&tpl=3&page=detail&type=top&topid=36&_=1520777874472").then(function(data){
//           console.log(data);
//       })
  }
};
</script>
<style scoped>
h1 {
  margin-top: 200px;
}
/* .container ul{
 padding: 0;
 margin: 0;
} */
.container ul li{
    position: relative;
    padding:10px;
    margin: 0;
    display: flex;

}
.container ul li img{
    width: 50px;
    height: 50px;
    margin-right: 10px;
}
.container ul li .next{
    position: absolute;
    top: 32px;
    right: 10px;
    border: 1px solid rgb(187, 183, 183);
    border-width: 0.1rem 0 0 0.1rem;
    width: 1rem;
    height: 1rem;
    -webkit-box-sizing: border-box;
    -webkit-transform-origin: 33.3% 33.3%;
    -webkit-transform: rotate(135deg);
    
}
</style>

