<template>
    <div class="section6 container">
        <div class="row1">
            <img class="img-left img-top" src="../assets/images/social-1.jpg" alt="">
            <div class="link">
                <div class="box">
                    <div class="text">Made for sharing</div>
                    <div class="title">Let's stay in touch</div>
                    <span class="button"><i class="fab fa-instagram"></i> Follow Us</span>
                </div>
            </div>
            <img class="img-right img-top" src="../assets/images/social-2.jpg" alt="">
        </div>
        <div class="row2">
            <img class="img-left img-bottom" src="../assets/images/social-3.jpg" alt="">
            <img class="img-center img-bottom" src="../assets/images/social-4.jpg" alt="">
            <img class="img-center img-bottom" src="../assets/images/social-5.jpg" alt="">
            <img class="img-right img-bottom" src="../assets/images/social-6.jpg" alt="">
        </div>
    </div>
</template>

<script>
export default {
    name: 'Section6'
}
</script>

<style scoped lang="scss">
.section6 {
    margin-bottom: 100px;
    .row1, .row2 {
        display: flex;
        flex-wrap: nowrap;
        .img-left {
            padding-right: 10px;
        }
        .img-center {
            padding-left: 10px;
            padding-right: 10px;
        }
        .img-right {
            padding-left: 10px;
        }
        .img-top {
            padding-bottom: 10px;
        }
        .img-bottom {
            padding-top: 10px;
        }
        img {
            width: calc(100% / 4);
        }
        .link {
            width: calc(100% / 2);
            height: 271,13px;
            margin-left: 10px;
            margin-right: 10px;
            margin-bottom: 10px;
            background-color: #F6F0F3;
            display: flex;
            justify-content: center;
            align-items: center;
            .box {
                text-align: center;
                .text {
                    font-size: 10px;
                    text-transform: uppercase;
                }
                .title {
                    color: #55338B;
                    font-size: 24px;
                    font-weight: 700;
                    margin-bottom: 20px;
                }
                .button {
                    color: white;
                    background-color: #55338B;
                    padding: 10px 20px;
                    border-radius: 5px;
                    cursor: pointer;
                }
            }
        }
    }
}
</style>