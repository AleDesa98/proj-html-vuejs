<template>
    <div class="section7">
        <div class="box">
            <div class="text">Try our seasonal products</div>
            <div class="title">Order for pick-up or delivery to your home</div>
            <span class="button">Shop Now</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Section7'
}
</script>

<style scoped lang="scss">
.section7 {
    height: 400px;
    background-image: url(../assets/images/call-to-action-bg.jpg);
    background-position: center center;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    display: flex;
    align-items: center;
    .box {
        position: absolute;
        left: 20%;
        width: 400px;
        .text {
            font-size: 10px;
            color: lightgray;
            text-transform: uppercase;
        }
        .title {
            color: white;
            font-size: 26px;
            font-weight: 700;
            margin-bottom: 50px;
        }
        .button {
            padding: 10px 20px;
            color: #585164;
            background-color: #FFFFFF;
            border-radius: 5px;
            cursor: pointer;
        }
    }
}
</style>