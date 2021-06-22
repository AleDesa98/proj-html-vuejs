<template>
    <div class="section1 container">
            <div class="left">
                <span>
                    Our products
                </span>
                <div>
                    All our delectable pastries are backed fresh in our Kitchen very morning, and are made with all-natural, all organic ingredients.
                </div>
                <span class="button">
                    Start Shopping
                </span>
            </div>
            <div class="center">
                <div class="black">
                    <div class="hover">
                        <div class="title">Choco Chip Cookies</div>
                        <div class="category">Cookies, Pastries</div>
                        <div class="price">$19.00 $39.00</div>
                    </div>
                </div>
            </div>
            <div class="right">
                <div class="black">
                    <div class="hover">
                        <div class="title">Strawberry Jam Cookies</div>
                        <div class="category">Cookies, Pastries</div>
                        <div class="price">$19.00 $39.00</div>
                    </div>
                </div>
            </div>
        </div>
</template>

<script>
export default {
    name: 'Section1'
}
</script>

<style scoped lang="scss">
.section1 {
    margin-top: 100px;
    margin-bottom: 100px;
    display: flex;
     & > .left {
        width: calc(100% /3 );
        height: 500px;
        & > span {
            font-size: 12px;
            color: grey;
            text-transform: uppercase;
        }
        & > div {
            color: #55338B;
            font-size: 28px;
            margin: 20px 0 60px 0;
        }
        & > .button {
            font-size: 1rem;
            color: white;
            padding: 15px 20px;
            background-color: #55338B;
            border-radius: 5px;
            cursor: pointer;
            text-transform: capitalize;
        }
        & > .button:hover {
            color: #55338B;
            background-color: lightgray;
        }
    }
    & > .center, .right {
        width: calc(100% /3 );
        background-position: center center;
        background-size: cover;
        background-repeat: no-repeat;
        margin: 0 10px;
        border-radius: 5px;
        .black {
            position: relative;
            width: 100%;
            height: 100%;
            border-radius: 5px;

            & > .hover {
                display: none;
                position: absolute;
                transform: translate(-50%, -50%);
                top: 50%;
                left: 50%;
                width: 100%;
                text-align: center;
                color: white;
                .title, .price {
                    font-size: 22px;
                }
                .category {
                    font-size: 14px;
                    margin-bottom: 10px;
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
    & > .center {
        background-image: url(../assets/images/choco-chip-cookies.jpg);
    }
    & > .right {
        background-image: url(../assets/images/strawberry-jam-cookies.jpg);
    }
}
</style>