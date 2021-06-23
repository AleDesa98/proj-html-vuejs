<template>
    <div class="section3 container">
        <div class="left">
            <div class="title">Find a freshly baked product perfect for you</div>
            <div class="text">Integer a nibh vitae ex porttitor ritrum et ut velit. Etiam ac felis at leo feugiat placerat. Sed ac nulla id orci tempor convallis sed.</div>
            <span class="button">Shop All Products</span>
        </div>
        <div class="right">
            <div class="item">
                <div class="product p1">
                    <div class="black">
                        <div class="hover">
                            <div class="hover-text">Select option / Quick view</div>
                        </div>
                    </div>
                </div>
                <div class="name">Choco Chip Cookies</div>
                <div class="price">$19.00 - $39.00</div>
            </div>
            <div class="item">
                <div class="product p2">
                    <div class="black">
                        <div class="hover">
                            <div class="hover-text">Select option / Quick view</div>
                        </div>
                    </div>
                </div>
                <div class="name">Strawberry Jam Cookies</div>
                <div class="price">$24.00 - $62.00</div>
            </div>
            <div class="item">
                <div class="product p3">
                    <div class="black">
                        <div class="hover">
                            <div class="hover-text">Select option / Quick view</div>
                        </div>
                    </div>
                </div>
                <div class="name">Strawberry Donut</div>
                <div class="price">$24.00 - $42.00</div>
            </div>
            <div class="item">
                <div class="product p4">
                    <div class="black">
                        <div class="hover">
                            <div class="hover-text">Select option / Quick view</div>
                        </div>
                    </div>
                </div>
                <div class="name">Perfect Macarons</div>
                <div class="price">$18.00 - $52.00</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Section3'
}
</script>

<style scoped lang="scss">
.section3 {
    display: flex;
    height: 300px;
    margin-top: 100px;
    margin-bottom: 250px;
    .left {
        width: 25%;
        text-align: center;
        height: 100%;
        padding-right: 20px;
        margin-top: 70px;
        .title {
            margin-top: 40px;
            color: #55338B;
            font-size: 24px;
        }
        .text {
            margin-top: 10px;
            margin-bottom: 30px;
            color: grey;
            font-size: 11px;
        }
        .button {
            margin-top: 20px;
            background-color: #55338B;
            padding: 10px 20px;
            color: white;
            border-radius: 5px;
            cursor: pointer;
        }
        .button:hover {
            background-color: lightgray;
            color: #55338B;
        }
    }
    .right {
        display: flex;
        width: 75%;
        height: 100%;
        .item {
            width: calc(100% / 4);
            // margin: 0 5px;
            margin-left: 10px;
            .p1 {
                background-image: url(../assets/images/choco-chip-cookies.jpg);
            }
            .p2 {
                background-image: url(../assets/images/strawberry-jam-cookies.jpg);
            }
            .p3 {
                background-image: url(../assets/images/strawberry-donut.jpg);
            }
            .p4 {
                background-image: url(../assets/images/perfect-macarons.jpg);
            }
            .product {
                width: 100%;
                height: 100%;
                background-position: center center;
                background-size: cover;
                background-repeat: no-repeat;
                border-radius: 5px;
                .black {
                    position: relative;
                    width: 100%;
                    height: 100%;
                    border-radius: 5px;
                    .hover {
                        display: none;
                        position: absolute;
                        transform: translate(-50%, -50%);
                        top: 50%;
                        left: 50%;
                        width: 100%;
                        text-align: center;
                        color: white;
                        .hover-text {
                            font-size: 14px;
                            text-transform: uppercase;
                        }
                    }
                }
                .black:hover .hover {
                    display: block;
                }
                .black:hover {
                    background-color: rgba($color: #000000, $alpha: 0.3);
                }
            }
            .name {
                text-align: center;
                color: #55338B;
                font-size: 18px;
                margin-top: 15px;
            }
            .price {
                text-align: center;
                font-size: 14px;
                color: #55338B;
                margin-top: 10px;
            }
        }
    }
}
</style>