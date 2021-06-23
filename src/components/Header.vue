<template>
    <header>
        <div class="menu">
            <div class="left">
                <img src="../assets/img/logo.svg" alt="">
            </div>
            <div class="right">
                <ul>
                    <LinkMenu 
                        v-for="(link, index) in links"
                        :key="index"
                        :text="link.testo"
                        :link="link.link"
                        :active="link.active"
                    />
                    <li><i class="fas fa-shopping-cart"></i></li>
                </ul>
            </div>
        </div>
        <section class="container">
            <span class="title">fresh & tasty bakery every day</span>
            <h1>The Perfect Fresh Bread</h1>
            <p>Cras consequant lectus vestibulum tortor pulvinar, quis euismod nisl varius. Aliquam erat volutpat. Nullam quis sagittis nibh ac nulla id orci tempor.</p>
            <span class="button">Explore our products</span>
        </section>
    </header>
</template>

<script>
import LinkMenu from './LinkMenu.vue'

export default {
    name: 'Header',
    components: {
        LinkMenu
    },
    props: ['links']
}
</script>

<style scoped lang="scss">
header {
    width: 100%;
    background-position: center center;
    background-size: cover;
    background-repeat: no-repeat;
    background-image: url(../assets/img/header.jpg);

    .menu {
        padding: 40px;
        height: 120px;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .left {
            & > img {
                height: 100%;
            }
        }
        .right > ul {
            display: flex;
            list-style: none;
            text-transform: uppercase;
            & > li {
                margin-left: 20px;
                color: #5b2ca2;
                padding-bottom: 5px;
                cursor: pointer;
            }
        }
    }
    section {
        padding: 120px 0 120px 0px;

        .title {
            text-transform: uppercase;
            font-size: 12px;
            color: grey;
            padding: 20px 0 20px 0;
        }
        h1 {
            color: #55338B;
            font-weight: 700;
            font-size: 45px;
            padding: 20px 0 20px 0;
        }
        p {
            color: grey;
            margin: 20px 0 40px 0;
            width: 500px;
        }
        .button {
            color: #55338B;
            padding: 10px 20px 10px 20px;
            background-color: white;
            border-radius: 5px;
            cursor: pointer;
        }
        .button:hover {
            color: white;
            background-color: #55338B;
        }
    }
}
</style>