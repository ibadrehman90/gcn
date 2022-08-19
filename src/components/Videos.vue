<template>

<div class="container">
  <div class="row">
    <div class="col-md-4 col-sm-12">
      <h3 class="latestVids">Latest Videos</h3>
      <VideoCard />
    </div>
  </div>
</div>
 
</template>

<script>
import VideoCard from '../components/VideoCard.vue'

export default {

    name:"Videos",
    components:{
    VideoCard
}
}
</script>

<style scoped>

.container{
  margin-top:20px;
}

.latestVids{
  padding:5px;
}

</style>