<template>
  <div class="hello">
    <div class="top">
      <img src="../assets/logo.png" alt="">
       <p>虾米音乐</p>
       <p>高品质试听下载，还能云收藏哦</p>
       <button>APP试听高品质</button>
    </div>
    <div class="nav">
     <p :class="{tab:Show==0}" @click="Show=0">新歌</p>
     <p :class="{tab:Show==1}" @click="Show=1">排行</p>
     <p :class="{tab:Show==2}" @click="Show=2">歌单</p>
     <p :class="{tab:Show==3}" @click="Show=3">歌手</p>
     <p :class="{tab:Show==4}" @click="Show=4">搜索</p>
     <br>
    </div>
    <New v-show="Show==0"></New>
    <Rankings v-show="Show==1"></Rankings>
    <List v-show="Show==2"></List>
    <Singer v-show="Show==3"></Singer>
    <Search v-show="Show==4"></Search>

    <!-- <New :is='shownav' keep-alive></New> -->
   
    <!-- <ul>
      <li>
        <a
          href="https://vuejs.org"
          target="_blank"
        >
          Core Docs
        </a>
      </li>
      <li>
        <a
          href="https://forum.vuejs.org"
          target="_blank"
        >
          Forum
        </a>
      </li>
      <li>
        <a
          href="https://chat.vuejs.org"
          target="_blank"
        >
          Community Chat
        </a>
      </li>
      <li>
        <a
          href="https://twitter.com/vuejs"
          target="_blank"
        >
          Twitter
        </a>
      </li>
      <br>
      <li>
        <a
          href="http://vuejs-templates.github.io/webpack/"
          target="_blank"
        >
          Docs for This Template
        </a>
      </li>
    </ul>
    <h2>Ecosystem</h2>
    <ul>
      <li>
        <a
          href="http://router.vuejs.org/"
          target="_blank"
        >
          vue-router
        </a>
      </li>
      <li>
        <a
          href="http://vuex.vuejs.org/"
          target="_blank"
        >
          vuex
        </a>
      </li>
      <li>
        <a
          href="http://vue-loader.vuejs.org/"
          target="_blank"
        >
          vue-loader
        </a>
      </li>
      <li>
        <a
          href="https://github.com/vuejs/awesome-vue"
          target="_blank"
        >
          awesome-vue
        </a>
      </li>
    </ul> -->
  
  </div>
</template>

<script>
import New from './new';
import Rankings from './rankings';
import List from './list';
import Singer from './singer';
import Search from './search';

export default {
  name: 'Home',
  data () {
    return {
     Show:0
    }
  },
  components:{
    New,
    Rankings,
    List,
    Singer,
    Search
  },
  // methods:{
  //   Show:function(tab){
  //     this.shownav=tab;

  //   }
  }
  

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.hello .top{
  width: 100%;
  height: 110px;
  background-color: #FF410F;
  position: relative;
  top: 0;
  left: 0;
}
.hello .top img{
  width: 40px;
  height: 45px;
  position: absolute;
  top: 35px;
  left: 10px; 
}
.hello .top p{
  margin-top: 0;
  color: white;
}
.hello .top p:nth-of-type(1){
  position: absolute;
  top: 37px;
  left: 55px;
  font-size: 15px;
}
.hello .top p:nth-of-type(2){
  position: absolute;
  top: 60px;
  left: 55px;
  font-size:10px;
}
.hello .top button{
  height: 35px;
  width: 130px;
  background-color: white;
  border:none;
  color: #FFAB7A;
  border-radius: 25px;
  position: absolute;
  top: 40px;
  right: 15px;
  font-size: 10px;
  /* font-weight: 600 */
}
.hello .nav{
  display: flex;
  justify-content: space-between;
  background-color: #F5F5F5
}
.hello .nav p{
  margin: 0;
  padding:15px 20px;
}
.hello .tab{
  color: #FF410F;
  border-bottom: 2px solid #FF410F
}
</style>
