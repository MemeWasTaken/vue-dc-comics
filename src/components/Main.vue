<template>
    <main>
        <div class="container-series">

        </div>
        <div class="merchandise">
            <div class="container">
                <ul class="merchandise-cards">
                    <li class="card">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        <div class="merch-text">Digital Comics</div>
                    </li>
                    <li class="card">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="">
                        <div class="merch-text">Dc Merchandise</div>
                    </li>
                    <li class="card">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                        <div class="merch-text">Subscription</div>
                    </li>
                    <li class="card">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                        <div class="merch-text">Comic Shop Locator</div>
                    </li>
                    <li class="card">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                        <div class="merch-text">Dc Power Visa</div>
                    </li>
                </ul>
            </div>
        </div>
    </main>
</template>

<script>
export default {
    name: 'Main',
}
</script>

<style lang="scss" scoped>
    main {

        .container-series {
            background-color: #1C1C1C;
            width: 100%;
            height: 104px;
        }
        .merchandise {
            background-color: #0282F9;
            width: 100%;
            height: 150px;

            .container {
                display: flex;
                justify-content: space-between;
                align-items: center;
                height: 150px;
                padding: 0 2em;

                .merchandise-cards {
                    display: flex;
                    justify-content: space-between;
                    align-items: center;
                    width: 100%;

                    .card {
                        display: flex;
                        align-items: center;

                        img {
                            width: 40px;
                            height: auto;
                        }

                        .merch-text {
                            color: #FFFFFF;
                            margin-left: 0.8em;
                            // font-weight: bold;
                            font-size: 0.9em;
                            text-transform: uppercase;

                        }
                    }
                }
            }
        }
    }
</style>