<template>
    <div class="container">
        <div class="search">
            <div class="form">
                <div class="keyafter">
                <input type="search" placeholder="输入歌曲、专辑、艺人名搜索" class="key">
                </div>
               <a class="btn-search">搜索</a>
            </div>
        </div>
        <div class="hot">
            <p>热门搜索</p> 
            <ul class="list">
                <li>
                    <a>抖音</a>
                </li>
                <li>
                    <a>纸短情长</a>
                </li>
                <li>
                    <a>9277</a>
                </li>
                <li>
                    <a>儿歌</a>
                </li>
                <li>
                    <a>陈奕迅</a>
                </li>
                <li>
                    <a>体面</a>
                </li>
                <li>
                    <a>张学友</a>
                </li>
                   <li>
                    <a>田馥甄</a>
                </li>
                   <li>
                    <a>空空如也</a>
                </li>
                   <li>
                    <a>张学友</a>
                </li>
                 <li>
                    <a>起风了</a>
                </li>
                 <li>
                    <a>后来</a>
                </li>
                 <li>
                    <a>戒烟</a>
                </li>


            </ul>
        </div>
    </div>
</template>
<script>
    export default{
        name:'search',

    }
</script>
<style scoped>
html{
    height: 100%;
    width: 100%;
}
body{
    height: 100%;
     width: 100%;
}
.container{
    width: 100%;
    height: 100%;
}
.container .search{
    /* height: 100%; */
    /* width: 100%; */
    padding: 10px;
    position: relative;
    border-bottom: 1px solid #D9D9D9;
}
/* .container .search .form { */
  /* display: flex;
  justify-content: space-around; */
  /* position: relative; */
/* } */
.container .search .form .keyafter {
    /* position: absolute; */
    width: 80%;
}
.container .search .form .keyafter::after{
    content: '';
    height: 18px;
    width: 18px;
    background-image: url(//gtms01.alicdn.com/tps/i1/TB1V1DqFVXXXXbMXpXX3pcaFFXX-25-25.png);
    background-size: 18px 18px;
    background-repeat: no-repeat;
    position: absolute;
    left: 20px;
    top: 21px;
}
.container .search .form .keyafter .key{
    width:100%;
    height: 40px;
    background-color: #F4F5F7;
    border: 0;
    border: 1px solid #D9D9D9;
    border-radius: 5px;
    padding-left:30px ;
    font-size: 13px;

}
.container .search .form .btn-search{
    position: absolute;
    top: 10px;
    right: 3px;
    height: 40px;
    line-height: 40px;
    width: 60px;
    text-align: center;
    font-size: 13px;
    color: white;
    border-radius: 5px;
    background-color: #fc9b0b;
    background-image: linear-gradient(to bottom ,#fda10d,#f77700)
}
.container .hot p{
    /* margin: 0; */
    text-align: left;
    margin-left: 10px;
    margin-top: 10px;
    font-size: 13px;
    color: #666666
}
.container .hot ul{
    text-align: left;
}
.container .hot ul li{
    display: inline-block;
    border: none;
    height: 32px;
    margin-left: 8px;
    margin-bottom: 8px;
    padding: 0 12px;
    font-size: 14px;
    line-height: 32px;
    color: #333;
    border: 1px solid #EBECEC;
    border-radius: 20px;

}

</style>

