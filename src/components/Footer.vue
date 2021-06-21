<template>
    <footer>
        <div class="top">
            <div class="left">
                <img src="../assets/img/logo.svg" alt="">
                <ul>
                    <LinkMenu 
                        v-for="(link, index) in links"
                        :key="index"
                        :text="link.testo"
                        :link="link.link"
                        :active="link.active"
                    />
                </ul>
            </div>
            <div class="right">
                <p>Subscribe to our Newsletter</p>
                <div class="newsletter">
                    <input type="text" placeholder="Enter email addres*">
                    <div class="button">Subscribe</div>
                </div>
            </div>
        </div>
        <div class="button">
            <div class="left"></div>
            <div class="right"></div>
        </div>
    </footer>
</template>

<script>
import LinkMenu from './LinkMenu.vue'

export default {
    name: 'Footer',
    components: {
        LinkMenu
    },
    props: ['links']
}
</script>

<style scoped lang="scss">
footer {
    width: 100%;

    .top {
        padding: 20px;
        display: flex;
        justify-content: space-between;

        .left {

            img {
                padding-left: 20px;
                padding-bottom: 30px;
            }
            ul {
                display: flex;
                list-style: none;
                text-transform: capitalize;
                margin-top: 20px;
            }
        }
        .right {
            width: 500px;
            p {
                padding-right: 20px;
                color: #55338B;
                font-size: 25px;
                text-align: right;
                padding-bottom: 30px;
            }
            .newsletter {
                display: flex;

                input {
                    flex-grow: 1;
                    border: 1px solid grey;
                    border-radius: 5px;
                    padding-left: 20px;
                }
                .button {
                    margin-right: 20px;
                    margin-left: 20px;
                    color: white;
                    padding: 15px 20px;
                    background-color: #55338B;
                    border-radius: 5px;
                    cursor: pointer;
                }
            }
        }
    }
}
</style>