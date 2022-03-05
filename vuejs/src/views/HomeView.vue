<template>
  <div class="home">
    <Sidebar />

    <div class="container">
      <div class="banner">
        <img src="@/assets/banner.png" alt="">
      </div>

      <div class="top-video">
        <Video v-for="video in listVideo" :vid="video" :key="video.id" />
      </div>
    </div>
  </div>
</template>

<script>
import Sidebar from "@/components/Sidebar.vue";
import Video from "@/components/Video.vue";

export default {
  name: "HomeView",
  components: {
    Sidebar,
    Video
  },
  data() {
    return {
      listVideo: [
        {
          id: 1,
          urlThumbnailImg: 'thumbnail1.png',
          urlOwnerImg: 'Jack.png',
          videoTitle: 'Best chanel to learn coding that help you to be a web developer',
          nameOwner: 'Easy Turtorials',
          views: '15k views',
          timeUpload: '2 days'
        },
        {
          id: 2,
          urlThumbnailImg: 'thumbnail2.png',
          urlOwnerImg: 'Jack.png',
          videoTitle: 'Best chanel to learn coding that help you to be a web developer',
          nameOwner: 'Easy Turtorials',
          views: '15k views',
          timeUpload: '2 days'
        },
        {
          id: 3,
          urlThumbnailImg: 'thumbnail3.png',
          urlOwnerImg: 'Jack.png',
          videoTitle: 'Best chanel to learn coding that help you to be a web developer',
          nameOwner: 'Easy Turtorials',
          views: '15k views',
          timeUpload: '2 days'
        },
        {
          id: 4,
          urlThumbnailImg: 'thumbnail4.png',
          urlOwnerImg: 'Jack.png',
          videoTitle: 'Best chanel to learn coding that help you to be a web developer',
          nameOwner: 'Easy Turtorials',
          views: '15k views',
          timeUpload: '2 days'
        },
        {
          id: 5,
          urlThumbnailImg: 'thumbnail5.png',
          urlOwnerImg: 'Jack.png',
          videoTitle: 'Best chanel to learn coding that help you to be a web developer',
          nameOwner: 'Easy Turtorials',
          views: '15k views',
          timeUpload: '2 days'
        },
        {
          id: 6,
          urlThumbnailImg: 'thumbnail6.png',
          urlOwnerImg: 'Jack.png',
          videoTitle: 'Best chanel to learn coding that help you to be a web developer',
          nameOwner: 'Easy Turtorials',
          views: '15k views',
          timeUpload: '2 days'
        },
        {
          id: 7,
          urlThumbnailImg: 'thumbnail7.png',
          urlOwnerImg: 'Jack.png',
          videoTitle: 'Best chanel to learn coding that help you to be a web developer',
          nameOwner: 'Easy Turtorials',
          views: '15k views',
          timeUpload: '2 days'
        },
        {
          id: 8,
          urlThumbnailImg: 'thumbnail8.png',
          urlOwnerImg: 'Jack.png',
          videoTitle: 'Best chanel to learn coding that help you to be a web developer',
          nameOwner: 'Easy Turtorials',
          views: '15k views',
          timeUpload: '2 days'
        },
      ]
    }
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
