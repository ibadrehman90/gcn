<template>

    <div :key="video._id" v-for="video in videoData">
        <div class="card" @click="goToVid(video.title)">
            <img :src="getImage(video._id)" />
            <div class="card-body">
                <p class="date">17th Auguest 2022</p>
                <p>{{video.title}}</p>
            </div>
        </div>
    </div>

</template>

<script>
import videoData from "../data.json";
export default {
    name: "VideoCard",
    data() {
        return {
            videoData: videoData
        }
    },
    methods: {
        getImage(id) {
            let image = "https://img.youtube.com/vi/" + id + "/mqdefault.jpg"
            return image
        },
        goToVid(title) {
            let str = title.toLowerCase().replace(/[^\w\s]/gi, '')
            let singleSpace = str.replace(/\s{2,}/g, ' ');
            let formattedStr = singleSpace.split(' ').join('-')
            let url = "https://www.globalcyclingnetwork.com/video/" + formattedStr
            window.location.href = url;
        }
    }
}
</script>

<style scoped>
.card {
    margin-bottom: 10px;
}

.date {
    font-weight: bold;
}

.card-body {
    padding: 10px;
}
</style>