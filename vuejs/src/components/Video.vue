<template>
  <div class="vid-item">
    <a href=""><img :src="require(`../assets/${vid.urlThumbnailImg}`)" alt="thumbnail" class="thumbnail"></a>
    <div class="flex-div">
      <img :src="require(`../assets/${vid.urlOwnerImg}`)" alt="">
      <div class="vid-info">
        <a href="">{{ vid.videoTitle }}</a>
        <p>{{ vid.nameOwner }}</p>
        <p>{{ vid.views }} &bull; {{ vid.timeUpload }}</p>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: "Video",
  props: ['vid'],
  methods: {
  },
};
</script>

<style>

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
