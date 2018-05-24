<template>
    <div class="container">
        <ul>
            <li>
                <p>华语男歌手</p>
                <div class="next"></div>
            </li>
            <li>
                <p>华语女歌手</p>
                <div class="next"></div>
            </li>
            <li>
                <p>华语乐队组合</p>
                <div class="next"></div>
            </li>
            <li>
                <p>欧美男歌手</p>
                <div class="next"></div>
            </li>
            <li>
                <p>欧美女歌手</p>
                <div class="next"></div>
            </li>
            <li>
                <p>欧美乐队组合</p>
                <div class="next"></div>
            </li>
              <li>
                <p>日本男歌手</p>
                <div class="next"></div>
            </li>
            <li>
                <p>日本女歌手</p>
                <div class="next"></div>
            </li>
            <li>
                <p>日本乐队组合</p>
                <div class="next"></div>
            </li>
            <li>
                <p>韩国男歌手</p>
                <div class="next"></div>
            </li>
            <li>
                <p>韩国女歌手</p>
                <div class="next"></div>
            </li>
            <li>
                <p>韩国乐队组合</p>
                <div class="next"></div>
            </li>
            
        </ul>
    </div>
</template>
<script>
export default {
  name: "singer"
};
</script>
<style scoped>
h1 {
  margin-top: 200px;
}
.container ul {
  padding: 0;
}
.container ul li {
  margin: 0;
  position: relative;
  height: 50px;
  padding: 10px;
}
.container ul li p {
  position: absolute;
}
.container ul li .next {
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

