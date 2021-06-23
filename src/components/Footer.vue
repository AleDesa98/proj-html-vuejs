<template>
    <footer>
        <div class="top container">
            <div class="left">
                <img src="../assets/img/logo.svg" alt="">
                <ul>
                    <LinkMenu 
                        v-for="(link, index) in links"
                        :key="index"
                        :text="link.testo"
                        :link="link.link"
                    />
                    <li>
                        <i class="fas fa-shopping-cart"></i>
                        <span>0</span>
                    </li>
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
        <div class="button container">
            <div class="left">
                <p>&#169; Copyright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress</p>
            </div>
            <div class="right">
                <ul>
                    <li><i class="fab fa-instagram"></i></li>
                    <li><i class="fab fa-twitter"></i></li>
                    <li><i class="fab fa-facebook-f"></i></li>
                    <li><i class="fab fa-pinterest-p"></i></li>
                </ul>
            </div>
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
    margin-top: 50px;
    .top {
        padding: 20px 0;
        display: flex;
        justify-content: space-between;

        .left {

            img {
                padding-bottom: 30px;
            }
            ul {
                display: flex;
                list-style: none;
                text-transform: capitalize;
                margin-top: 20px;
                margin-left: -20px;
                padding-left: 0;
                & > li {
                    margin-left: 20px;
                    color: #5b2ca2;
                    padding-bottom: 5px;
                    cursor: pointer;
                    & > span {
                        background-color: #F1EDF4;
                        border-radius: 50%;
                        margin-left: 3px;
                        padding: 3px;
                    }
                }
            }
        }
        .right {
            width: 500px;
            p {
                color: #55338B;
                font-size: 25px;
                text-align: right;
                padding-bottom: 10px;
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
                    margin-left: 20px;
                    color: white;
                    padding: 10px 20px;
                    background-color: #55338B;
                    border-radius: 5px;
                    cursor: pointer;
                }
            }
        }
    }
    .button {
        padding: 40px 0;
        display: flex;
        justify-content: space-between;
        .left {
            p {
                font-size: 12px;
                color: grey;
            }
        }
        .right {
            ul {
                list-style: none;
                display: flex;

                li {
                    margin-left: 40px;
                    color: #55338B;
                    cursor: pointer;
                }
            }
        }
    }
}
</style>