<template>
    <main>
        <div class="label">current series</div>
    </main>
</template>

<script>
export default {
    
}
</script>

<style lang="scss">
@import '@/style/variables.scss';

main{
    position: relative;
    height: 100px;
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

}
</style>