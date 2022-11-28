<template>
    <div>
        <header-sito></header-sito>
        <main-page></main-page>
        <footer-page></footer-page>
    </div>
</template>

<script>
import HeaderSito from './components/HeaderSito.vue';
import MainPage from './components/MainPage.vue';
import FooterPage from '@/components/FooterPage.vue'

export default {
    components: {
        HeaderSito,
        MainPage,
        FooterPage,
    },
}

</script>
<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@400;500;600&display=swap');
@import 'https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/all.min.css';
    *{
        padding: 0;
        margin: 0;
        box-sizing: border-box;
    }
    html{
        font-family: 'Oswald', sans-serif;

    }
</style>