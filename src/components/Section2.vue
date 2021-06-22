<template>
    <div class="section2 container">
            <div class="top text-center">
                <div class="category">Corporate & Weddings</div>
                <div class="title">Baking Special Moments</div>
            </div>
            <div class="botton">
                <div class="left">
                    <div class="hover">
                        <div class="category">International bakery</div>
                        <div class="title">Corporate Events</div>
                        <span class="button">Explore more</span>
                    </div>
                </div>
                <div class="right">
                    <div class="hover">
                        <div class="category">Private dining hall</div>
                        <div class="title">Weddings & Parties</div>
                        <span class="button">Explore more</span>
                    </div>
                </div>
            </div>
        </div>
</template>

<script>
export default {
    name:'section2'
}
</script>

<style scoped lang="scss">
.section2 {
    margin-bottom: 50px;
    .top {
        padding-top: 60px;
        & > .category {
            font-size: 12px;
            color: grey;
            text-transform: uppercase;
        }
        & > .title {
            color: #55338B;
            font-size: 28px;
            margin: 10px 0 60px 0;
        }
    }
    .botton {
        display: flex;
        justify-content: space-between;
        height: 600px;
        .left, .right {
            position: relative;
            width: calc(50% - 30px);
            height: 100%;
            background-position: center center;
            background-size: cover;
            background-repeat: no-repeat;
            border-radius: 5px;

            .hover {
                display: none;
                position: absolute;
                transform: translate(-50%, -50%);
                top: 50%;
                left: 50%;
                text-align: center;

                .category {
                    font-size: 10px;
                    color: lightgray;
                    text-transform: uppercase;
                }
                .title {
                    font-size: 26px;
                    color: white;
                    margin: 10px 0 20px 0;
                }
                .button {
                    font-size: 14px;
                    color: white;
                    background-color: #55338B;
                    padding: 10px 20px;
                    border-radius: 5px;
                    cursor: pointer;
                }
                .button:hover {
                    background-color: lightgray;
                    color: #55338B;
                }
            }
            .hover:hover {
                display: block;
            }

        }
        .left {
            background-image: url(../assets/images/corporate-bg.jpg);
        }
        .left:hover {
              background-image: url(../assets/images/corporate-hover-bg.jpg);
        }
        .left:hover .hover {
            display: block;
        }
        .right {
            background-image: url(../assets/images/wedding-bg.jpg);
        }
        .right:hover {
              background-image: url(../assets/images/wedding-hover-bg.jpg);
        }
        .right:hover .hover {
            display: block;
        }
    }
}
</style>