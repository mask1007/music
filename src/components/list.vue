<template>
    <div class="container">
       <ul>
           <li>
                <img src="http://pic.xiami.net/images/collect/40/40/392795040_5aebe728c57ba_oAt0_1525409576.jpg" alt="">
                <p>初夏晚歌。</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="http://pic.xiami.net/images/trade/common/2410/5a01077c975d9_120522600_b_w700h700_face_w700h700_x257y408w58h73c1.jpg" alt="">
                <p>触摸灵魂的20首冷门小众英文歌（女声篇）</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="http://pic.xiami.net/images/collect/564/64/358483564_1526354940_qIeH.jpg" alt="">
                <p>我最喜欢港乐系列</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="http://img.xiami.net/images/appv5/common/9707/5acd632be8edf_zIWx_1523409707.jpg" alt="">
                <p>女团抒情篇(愿托乔木伴你青)</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="http://pic.xiami.net/images/collect/701/1/356338701_5afa5f0d05e6b_gTRv_1526357773.jpg" alt="">
                <p>欧美女声‖ 百里不如挑一，只求天赋好嗓</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="http://pic.xiami.net/images/collect/26/26/364576026_5adc33a8eb8c3_bojJ_1524380584.jpg" alt="">
                <p>一人一首华语R&B（男声篇）</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="http://pic.xiami.net/images/collect/24/24/261964024_1526131995_q5qV.jpg" alt="">
                <p>欧美女声‖ 百里不如挑一，只求天赋好嗓</p>
                <div class="next"></div>
            </li>
            <li>
                <img src="http://pic.xiami.net/images/collect/888/88/355387888_1507367941_UiBu.png" alt="">
                <p>走进粤语流行放音室</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="http://pic.xiami.net/images/collect/784/84/394048784_5aec648b60d77_N9aa_1525441675.jpg" alt="">
                <p>听了n年才知歌名系列</p>
                <div class="next"></div>
            </li>
             <li>
                <img src="http://pic.xiami.net/images/common/uploadpic/playlist/271065482/1526747829589.jpeg" alt="">
                <p>520告白季，用歌名连句去表白</p>
                <div class="next"></div>
            </li>
       </ul>
    </div>
</template>
<script >
export default {
  name: "list"
};
</script>
<style scoped>
h1 {
  margin-top: 200px;
}
.container ul{
 padding: 0;
}
.container ul li {
  height: 50px;
  padding: 10px;
  margin: 0;
  position: relative;
}
.container ul li img {
  width: 50px;
  height: 50px;
  left: 15px;
  position: absolute;
}
.container ul li p {
  position: absolute;
  text-align: left;
  margin-left: 60px;
  width: 250px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
.container ul li .next {
  position: absolute;
  border: 1px solid rgb(187, 183, 183);
  border-width: 0.1rem 0 0 0.1rem;
  width: 1rem;
  height: 1rem;
  -webkit-box-sizing: border-box;
  -webkit-transform-origin: 33.3% 33.3%;
  -webkit-transform: rotate(135deg);
  top: 32px;
  right: 10px;
}
</style>

