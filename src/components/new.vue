<template>
    <div class="container">
        <a href="http://m.xiami.com/dl?ch=700828"><img src="//gw.alicdn.com/tps/TB1s.XCKFXXXXbRXFXXXXXXXXXX-750-176.png" alt=""></a>
        
        <ul>
            <li v-for="i in item" :key="i.id" class="list">
              <p class="songname">{{i.data.albumname}}</p>
              <p class="singername">{{i.data.singer[0].name}}</p>
            </li>
        </ul>
    </div>
</template>
<script>
import axios from "axios";
export default {
  name: "new",
  data: function() {
    return {
      item: []
    };
  },
  mounted: function() {
    console.log("---------");
    axios
      .get(
        "https://c.y.qq.com/v8/fcg-bin/fcg_v8_toplist_cp.fcg?g_tk=5381&uin=0&format=json&inCharset=utf-8&outCharset=utf-8&notice=0&platform=h5&needNewCode=1&tpl=3&page=detail&type=top&topid=27&_=1519963122923"
      )
      .then(
        function(data) {
          //   console.log(data);
          console.log(data.data);
          this.item = data.data.songlist;
          console.log(this.item);
        }.bind(this)
      )
      .catch(function(response) {
        console.log(response);
      });
  }
};
</script>
<style>
h1 {
  margin-top: 200px;
}
.container img {
  width: 100%;
}
.container ul {
  padding: 0;
  margin: 0;
}
.container ul li {
  list-style: none;
  border-bottom: 2px solid #f5f5f5;
  padding-left: 15px;
}
.container ul li .songname {
  text-align: left;
  margin-bottom: 2px;
  margin-top: 10px;
  font-size: 15px
}
.container ul li .singername {
  text-align: left;
  margin-top: 0px;
  margin-bottom: 10px;
  font-size: 12px;
  color: #AFAFB0
}
</style>

