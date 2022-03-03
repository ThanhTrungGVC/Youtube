<template>
  <div class="home">
    <Sidebar />

    <div class="container">
      <div class="banner">
        <img src="@/assets/banner.png" alt="">
      </div>

      <div class="top-video">
        <div class="vid-item">
          <a href=""><img src="@/assets/thumbnail1.png" alt="" class="thumbnail"></a>
          <div class="flex-div">
            <img src="@/assets/Jack.png" alt="">
            <div class="vid-info">
              <a href="">Best chanel to learn coding that help you to be a web developer</a>
              <p>Easy Turtorials</p>
              <p>15k views &bull; 2 days</p>
            </div>
          </div>
        </div>

        <div class="vid-item">
          <a href=""><img src="@/assets/thumbnail2.png" alt="" class="thumbnail"></a>
          <div class="flex-div">
            <img src="@/assets/Jack.png" alt="">
            <div class="vid-info">
              <a href="">Best chanel to learn coding that help you to be a web developer</a>
              <p>Easy Turtorials</p>
              <p>15k views &bull; 2 days</p>
            </div>
          </div>
        </div>

        <div class="vid-item">
          <a href=""><img src="@/assets/thumbnail3.png" alt="" class="thumbnail"></a>
          <div class="flex-div">
            <img src="@/assets/Jack.png" alt="">
            <div class="vid-info">
              <a href="">Best chanel to learn coding that help you to be a web developer</a>
              <p>Easy Turtorials</p>
              <p>15k views &bull; 2 days</p>
            </div>
          </div>
        </div>

        <div class="vid-item">
          <a href=""><img src="@/assets/thumbnail4.png" alt="" class="thumbnail"></a>
          <div class="flex-div">
            <img src="@/assets/Jack.png" alt="">
            <div class="vid-info">
              <a href="">Best chanel to learn coding that help you to be a web developer</a>
              <p>Easy Turtorials</p>
              <p>15k views &bull; 2 days</p>
            </div>
          </div>
        </div>

        <div class="vid-item">
          <a href=""><img src="@/assets/thumbnail5.png" alt="" class="thumbnail"></a>
          <div class="flex-div">
            <img src="@/assets/Jack.png" alt="">
            <div class="vid-info">
              <a href="">Best chanel to learn coding that help you to be a web developer</a>
              <p>Easy Turtorials</p>
              <p>15k views &bull; 2 days</p>
            </div>
          </div>
        </div>

        <div class="vid-item">
          <a href=""><img src="@/assets/thumbnail6.png" alt="" class="thumbnail"></a>
          <div class="flex-div">
            <img src="@/assets/Jack.png" alt="">
            <div class="vid-info">
              <a href="">Best chanel to learn coding that help you to be a web developer</a>
              <p>Easy Turtorials</p>
              <p>15k views &bull; 2 days</p>
            </div>
          </div>
        </div>

        <div class="vid-item">
          <a href=""><img src="@/assets/thumbnail7.png" alt="" class="thumbnail"></a>
          <div class="flex-div">
            <img src="@/assets/Jack.png" alt="">
            <div class="vid-info">
              <a href="">Best chanel to learn coding that help you to be a web developer</a>
              <p>Easy Turtorials</p>
              <p>15k views &bull; 2 days</p>
            </div>
          </div>
        </div>

        <div class="vid-item">
          <a href=""><img src="@/assets/thumbnail8.png" alt="" class="thumbnail"></a>
          <div class="flex-div">
            <img src="@/assets/Jack.png" alt="">
            <div class="vid-info">
              <a href="">Best chanel to learn coding that help you to be a web developer</a>
              <p>Easy Turtorials</p>
              <p>15k views &bull; 2 days</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Sidebar from "@/components/Sidebar.vue";

export default {
  name: "HomeView",
  components: {
    Sidebar,
  },
};
</script>

<style>

.home {
  width: 100%;
  height: 100%;
}

.home .container{
  margin-left: 15%;
  width: 84%;
  height: 100%;
  background: #f9f9f9;
  padding: 20px 2% 20px 2%;
  overflow: auto;
}

.banner {
  width: 100%;
}

.banner img{
  width: 100%;
  border-radius: 8px;
}

.top-video{
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  grid-column-gap: 16px;
  grid-row-gap: 30px;
  margin-top: 15px;
  margin-bottom: 10px;
}

/* width */
::-webkit-scrollbar {
  width: 10px;
}

/* Track */
::-webkit-scrollbar-track {
  background: #f1f1f1; 
}
 
/* Handle */
::-webkit-scrollbar-thumb {
  background: #888; 
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #555; 
}

.vid-item .thumbnail{
    width: 100%;
    border-radius: 5px;
}

.vid-item .flex-div{
    align-items: flex-start;
    margin-top: 7px;
    display: flex;
}

.vid-item .flex-div img{
    width: 35px;
    margin-right: 10px;
    border-radius: 50%;
}

.vid-info{
    color: #5a5a5a;
    font-size: 13px;
}

.vid-info a{
    color: #000;
    font-weight: 600;
    display: block;
    margin-bottom: 5px;
}

</style>
