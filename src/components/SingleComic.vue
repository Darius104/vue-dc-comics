<template>
    <div>
        <div>
            <img :src="element.thumb" :alt="element.series">
        </div>

        <div class="title">
            {{ element.series.toUpperCase() }}
        </div>
    </div>
</template>

<script>
export default {
    name: 'SingleComic',
    props:['element'],
}
</script>

<style lang="scss" scoped>
    .title{
        color: white;
    }
</style>