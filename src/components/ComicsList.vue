<template>
    <div class="back">
        <div class="container">
            <SingleComic v-for="(e, index) in list" :key="index" :element = "e"/>
        </div>
    </div>
</template>

<script>
import './SingleComic.vue';
export default {
    name: "ComicsList",
    components: { SingleComic },
}
</script>

<style lang="scss" scoped>
@import '../style/Commun.scss';
    .back{
        background: gray;

        ul{
            list-style-type: none;
            display: flex;
            flex-wrap: wrap;

            li{
                width: calc(100% / 6);
                padding: 20px;
                margin-top: 40px;
            }
        }
    }
    
</style>