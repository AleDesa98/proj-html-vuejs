<template>
    <div class="section5 container">
        <div class="top text-center">
            <div class="category">Locations</div>
            <div class="title">Visit our Bakeries</div>
        </div>
        <div class="bottom">
            <div class="left">
                <div class="image"></div>
                <div class="place">
                    <div class="name">New York</div>
                    <div class="description">
                        <div class="number">
                            <div class="text">Call us</div>
                            <div class="contact">1.800.458.556</div>
                        </div>
                        <div class="open-day">
                            <div class="text">Open all week</div>
                            <div class="contact">9.00 AM - 6:00 PM</div>
                        </div>
                        <div class="button">
                            <span>View Map</span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="right">
                <div class="image"></div>
                <div class="place">
                    <div class="name">London</div>
                    <div class="description">
                        <div class="number">
                            <div class="text">Call us</div>
                            <div class="contact">1.800.458.556</div>
                        </div>
                        <div class="open-day">
                            <div class="text">Open all week</div>
                            <div class="contact">9.00 AM - 6:00 PM</div>
                        </div>
                        <div class="button">
                            <span>View Map</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Section5'
}
</script>

<style scoped lang="scss">
.section5 {
    margin-bottom: 100px;
    .top {
        padding-top: 150px;
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
    .bottom {
        width: 100%;
        display: flex;
        & > .left {
            & > .image {
                background-image: url(../assets/images/new-york-bk.jpg);
            }
            & > .place {
                background-color: #F0F9FB;
            }
        }
        & > .right {
            & > .image {
                background-image: url(../assets/images/london-bk.jpg);
            }
            & > .place {
                background-color: #FAF3E3;
            }
        }
        .left, .right {
            width: 50%;
            .image {
                width: 100%;
                height: 400px;
                background-position: center center;
                background-size: cover;
                background-repeat: no-repeat;
            }
            .place {
                width: 100%;
                padding-bottom: 20px;
                .name {
                    color: #55338B;
                    text-align: center;
                    padding: 20px 0;
                    font-size: 22px;
                    font-weight: 500;
                }
                .description {
                    display: flex;
                    justify-content: space-around;
                    align-items: center;
                    text-align: center;
                    .number, .open-day, .button {
                        width: calc(100% / 3);
                    }
                    .number, .open-day {
                        color: grey;
                        .text {
                            font-size: 10px;
                            text-transform: uppercase;
                        }
                        .contact {
                            font-size: 14px;
                        }
                    }
                    .button > span {
                        background-color: white;
                        color: #55338B;
                        padding: 10px 20px;
                        border-radius: 5px;
                        cursor: pointer;
                    }
                    .button > span:hover {
                        color: white;
                        background-color: #55338B;
                    }
                }
            }
        }
    
    }
}
</style>