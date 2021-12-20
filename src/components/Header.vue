<template>
    <header>
        <div class="container">
            <div>
                <img src="../assets/img/dc-logo.png" alt="Logo principale">
            </div>

            <ul >
                <li v-for="(element, index) in links" :key="index"><a href="">{{ links[index].content }}</a></li>
            </ul>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    data: function(){
        return {
            links: [
                {
                    content: 'CHARACTERS',
                    url: '#',
                    active: false
                },
                {
                    content: 'COMICS',
                    url: '#',
                    active: true
                },
                {
                    content: 'MOVIES',
                    url: '#',
                    active: false
                },
                {
                    content: 'TV',
                    url: '#',
                    active: false
                },
                {
                    content: 'GAMES',
                    url: '#',
                    active: false
                },
                {
                    content: 'COLLECT',
                    url: '#',
                    active: false
                },
                {
                    content: 'VIEDO',
                    url: '#',
                    active: false
                },
                {
                    content: 'FANS',
                    url: '#',
                    active: false
                },
                {
                    content: 'NEWS',
                    url: '#',
                    active: false
                },
                {
                    content: 'SHOP',
                    url: '#',
                    active: false
                }
            ],
        }
    }
}
</script>

<style scoped lang="scss">
@import '../style/ColorApp.scss';
    .container{
        width: 100%;
        height: 150px;
        display: flex;
        justify-content: center;
        align-items: center;
        justify-content: space-around;

        img{
            width: 90px;
        }
        ul{
            list-style-type: none;
            display: flex;            
            align-items: center;

            li{
                margin: 0 20px;

                a{
                    padding: 55px 0;
                    text-decoration: none;
                    color: gray;
                    font-weight: bold; 

                    &:hover{
                        border-bottom: 8px solid $color_style;
                    }
                }
            }
        }
    }
</style>