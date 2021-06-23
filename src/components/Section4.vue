<template>
    <div class="section4 container">
        <div class="row1">
            <div class="black"></div>
            <div class="title">Tell us what you have in mind</div>
            <div class="number">01</div>
            <div class="description">
                <div class="name">Manual ingredients selection</div>
                <div class="text">Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat, finibus in velit placerat, rutrum augue.</div>
            </div>
        </div>
        <div class="row2">
            <div class="img">
                <div class="black"></div>
                <div class="title">We Start Baking</div>
                <div class="number">02</div>
                <div class="description">
                    <div class="name">Sweet & Delicious</div>
                    <div class="text">Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat, finibus in velit placerat.</div>
                </div>
            </div>
            <div class="text">
                <div class="box">
                    <div class="description">Dont just take our word for it</div>
                    <div class="text">"Finally found an alternative to the mass produced products. Something that incorporates real organic ingredients, nutrient dense wellness while promoting sustainability and activity."</div>
                    <div class="author">Rachel Cooper, Founder</div>
                </div>
            </div>
        </div>
        <div class="row3">
            <div class="black"></div>
            <div class="title">Delivered to your home</div>
            <div class="number">03</div>
            <div class="description">
                <div class="name">Baked to order & gift wrapped</div>
                <div class="text">Cras consequat lectus vestibulum tortor pulvinar, quis euismod nisl varius. Ut eu laoreet ex. Aliquam erat volutpat. Nullam quis sagittis nibh. Morbi consectetur ultricies ante ac congue. Donec lorem erat, finibus in velit placerat, rutrum augue.</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Section4'
}
</script>

<style scoped lang="scss">
.row1 {
    width: 100%;
    height: 500px;
    background-image: url(../assets/images/bakery-process-1.jpg);
    background-position: center center;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    color: white;
    & > .black {
        position: absolute;
        width: 100%;
        height: 100%;
        background-color: rgba($color: #000000, $alpha: 0.3);
    }
    & > .title {
        position: absolute;
        top: 50px;
        left: 60px;
        font-size: 36px;
        font-weight: 700;
        width: 400px;
        line-height: 50px;
    }
    & > .number {
        position: absolute;
        top: 50px;
        right: 60px;
        font-weight: 100;
        font-size: 60px;
    }
    & > .description {
        position: absolute;
        width: 450px;
        bottom: 50px;
        right: 60px;
        & > .name {
            text-transform: uppercase;
            color: lightgray;
            font-size: 10px;
            margin-bottom: 10px;
        }
        & > .text {
            font-size: 16px;
        }
    }
}
.row2 {
    display: flex;
    justify-content: space-between;
    height: 500px;
    margin-top: 20px;
    margin-bottom: 20px;
    & > .img {
        position: relative;
        width: 50%;
        height: 100%;
        margin-right: 10px;
        background-image: url(../assets/images/bakery-process-2.jpg);
        background-position: center center;
        background-size: cover;
        background-repeat: no-repeat;
        color: white;
        & > .black {
            position: absolute;
            width: 100%;
            height: 100%;
            background-color: rgba($color: #000000, $alpha: 0.3);
        }
        & > .title {
            position: absolute;
            top: 50px;
            left: 60px;
            font-size: 36px;
            font-weight: 700;
            width: 400px;
            line-height: 50px;
        }
        & > .number {
            position: absolute;
            top: 35px;
            right: 60px;
            font-weight: 100;
            font-size: 60px;
        }
        & > .description {
            position: absolute;
            width: 320px;
            bottom: 50px;
            left: 60px;
            & > .name {
                text-transform: uppercase;
                color: lightgray;
                font-size: 10px;
                margin-bottom: 10px;
            }
            & > .text {
                font-size: 16px;
            }
        }
    }
    & > .text {
        width: 50%;
        height: 100%;
        background-color: lightgray;
        margin-left: 10px;
        padding: 50px;
        display: flex;
        align-items: center;
        & > .box {
            & > .description {
                font-size: 10px;
                text-transform: uppercase;
            }
            & > .text {
                font-size: 30px;
                line-height: 45px;
                margin: 20px 0;
                color: #55338B;
                font-weight: 700;
            }
            & > .author {
                font-size: 10px;
            }
        }
    }
}
.row3 {
    width: 100%;
    height: 500px;
    background-image: url(../assets/images/bakery-process-3.jpg);
    background-position: center center;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    color: white;
    & > .black {
        position: absolute;
        width: 100%;
        height: 100%;
        background-color: rgba($color: #000000, $alpha: 0.3);
    }
    & > .title {
        position: absolute;
        top: 50px;
        left: 60px;
        font-size: 36px;
        font-weight: 700;
        width: 400px;
        line-height: 50px;
    }
    & > .number {
        position: absolute;
        top: 50px;
        right: 60px;
        font-weight: 100;
        font-size: 60px;
    }
    & > .description {
        position: absolute;
        width: 450px;
        bottom: 50px;
        left: 60px;
        & > .name {
            text-transform: uppercase;
            color: lightgray;
            font-size: 10px;
            margin-bottom: 10px;
        }
        & > .text {
            font-size: 16px;
        }
    }
}
</style>