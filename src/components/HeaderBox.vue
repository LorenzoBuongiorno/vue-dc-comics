<template>
    <header>
        <div class="header-container">
            <div class="logo">
                <img src="@/assets/img/dc-logo.png" alt="">
            </div>
            <ul>
                <li v-for="button in nav" :key="button.id">
                    <a :href="button.url">{{button.label}}</a>
                </li>
            </ul>
        </div>
    </header>
</template>

<script>
export default {
    props: {
        nav: Array
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
@import '@/style/header.scss';
</style>