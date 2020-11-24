<template>
    <h2>concept</h2>
    <figure class="concept-figure"><img src="@/assets/concept_figure.png" alt=""></figure>
    <p class="concept-description">FACTORY=SHOP<br>THE FINEST INGREDIENTS FROM ENGLAND</p>
    <section class="concept-item">
        <h3 class="concept-item-title">挽きたてフレッシュな美味しさを目の前で。<br>英国生まれのうさショコラ</h3>
        <p class="concept-item-description">ガトーショコラの中身にこだわるのは、ごく普通。「普通のガトーショコラに意外性をもたせたい」という発想から、うさぎを練り込んガトーショコラが生まれました。焼きたての味を届けたいから、工房一体型の店舗で全て焼き上げてご提供しています。</p>
    </section>
</template>

<script>
export default {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">

    .concept-title {
        font-size: 72px;
        line-height: 46px;
        padding-top: 55px;
        font-family: 'Quicksand', sans-serif;
        font-style: normal;
        font-weight: bold;
    }

    .concept-description {
        font-family: Quicksand;
        font-style: normal;
        font-weight: normal;
        padding-top: 45px;
        font-size: 48px;
        line-height: 46px;
    }

    .concept-figure {
        padding-top: 62px;
    }

    .concept-item {
        padding-top: 110px;
    }

    .concept-item-title {
        font-family: Mplus 1p;
        font-style: normal;
        font-weight: normal;
        font-size: 22px;
        line-height: 40px;
    }

    .concept-item-description {
        padding-top: 25px;
        width: 600px;
        margin-right: auto;
        margin-left: auto;
        font-family: Mplus 1p;
        font-style: normal;
        font-weight: normal;
        font-size: 14px;
        line-height: 23px;
    }
</style>