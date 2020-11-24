<template>
    <h2 class="what-title"><span class="what-title-mini">WHAT IS</span>USA CHOCOLATE</h2>
    <div class="what-container">
        <dl class="what-item">
            <dt class="what-choco-figure"><img src="@/assets/what_usagi.png" alt="" class="what-choco-figure-img"></dt>
            <dd class="what-choco-description">HUWAHUWA EAR</dd>
        </dl>
        <dl class="what-item">
            <dt class="what-usagi-figure"><img src="@/assets/what_realusagi.png" alt="" class="what-usagi-figure-img"></dt>
            <dd class="what-usagi-description">REAL USAGI</dd>
        </dl>
        <dl class="what-item">
            <dt class="what-ribon-figure"><img src="@/assets/what_ribon.png" alt="" class="what-ribon-figure-img"></dt>
            <dd class="what-ribon-description">かわいくおめかしするためにつけた<br>国産のピンクのリボン</dd>
        </dl>
    </div>
</template>

<script>
export default {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
    .what-title {
        padding-top: 145px;
        font-family: Quicksand;
        font-style: normal;
        font-weight: bold;
        font-size: 100px;
        white-space: nowrap;
    }

    .what-title-mini {
        top: 100px;
        right: 50%;
        transform: translateX(50%);
        position: absolute;
        font-family: Quicksand;
        font-style: normal;
        font-weight: bold;
        font-size: 48px;
        line-height: 63px;
        color: #FAFF00;
    }
    
    .what-container {
        width: 960px;
        height: 345px;
        margin-top: 80px;
        position: relative;
        margin-right: auto;
        margin-left: auto;
    }

    .what-choco-description {
        font-family: Quicksand;
        font-style: normal;
        font-weight: normal;
        font-size: 24px;
        top: 0;
        left: 0;
        line-height: 43px;
        position: absolute;
        &:before {
            content: "";
            display: block;
            width: 270px;
            border-style: solid none none none;
            border-color: white;
            border-width: 1px;
            position: absolute;
            top: 20px;
            left: 220px;
        }
        &:after {
            content:"";
            position: absolute;
            background-color: white;
            left: 218px;
            top: 13px;
            display: block;
            width: 15px;
            height: 15px;
            border-radius: 50%;
        }
    }

    .what-usagi-description {
        font-family: Quicksand;
        font-style: normal;
        font-weight: normal;
        font-size: 24px;
        line-height: 43px;
        position: absolute;
        right: 0;
        &:before {
            content: "";
            display: block;
            width: 45px;
            height: 227px;
            border: 1px solid;
            border-color: white transparent white white;
            position: absolute;
            top: 20px;
            left: -50px;
        }
        &:after {
            content:"";
            position: absolute;
            background-color: white;
            display: block;
            top: 13px;
            left: -18px;
            width: 15px;
            height: 15px;
            border-radius: 50%;
        }
    }

    .what-ribon-description {
        font-family: Mplus 1p;
        font-style: normal;
        font-weight: normal;
        font-size: 12px;
        line-height: 22px;
        text-align: left;
        position: absolute;
        top: 230px;
        left: 0;
    }

    .what-choco-figure-img {
        position: absolute;
        right: 50%;
        top: 0;
        transform: translateX(50%);
    }

    .what-usagi-figure-img {
        position: absolute;
        right: 0;
        bottom: 0;
    }

    .what-ribon-figure-img {
        position: absolute;
        bottom: 0;
        left: 48px;
    }
</style>