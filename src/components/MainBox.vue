<template>
    <main>
        <div class="label">current series</div>
        <ul>
            <li v-for="(item, i) in cards" :key="i">
                <a href="#">
                    <div class="picture">
                        <img :src="item.thumb" alt="">
                    </div>
                    <div class="name-series">{{item.series}}</div>
                </a>
            </li>
        </ul>
        <div class="load-more"><a href="#">load more</a></div>
    </main>
</template>

<script>
export default {
    props: {
        cards: Array
    }
    
}
</script>

<style lang="scss">
@import '@/style/variables.scss';

main{
    background-color: #222;
    position: relative;
    .label{
        position: absolute;
        top: -20px;
        left: 200px;
        padding: 10px 30px;
        color: $text-light-color;
        font-size: 30px;
        font-weight: bold;
        background-color: $main-color;
        text-transform: uppercase;
    }
    ul{
        padding: 50px;
        width: 1600px;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
        li{
            padding: 10px;
            width: calc(100% / 6);
            .picture{
                height: 220px;
                img{
                    width:100%;
                    height: 100%;
                    object-fit:cover;
                    object-position: top;
                }
            }
            .name-series{
                margin-top: 15px;
                color:$text-light-color;
                text-transform: uppercase;
                font-size: 20px;
            }
        }
    }
    .load-more{
        text-align: center;
        padding-bottom: 60px;
        a{
            padding: 15px 80px;
            background-color: $main-color;
            color:$text-light-color;
            text-transform: uppercase;
            font-weight: bold;
            font-size: 20px;
        }
    }

}
</style>