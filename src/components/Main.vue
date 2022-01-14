<template>
    <main>
        
        <div class="jumbo">

        </div>

        <div class="container-series">
            <div class="container">
                <h2> Current Series </h2>
                <Series 
                    v-for="(serie, index) in series"
                    :key="index"
                    :img="serie.thumb"
                    :title="serie.series"
                />
            </div>
               <div> <a href="#">Load More</a> </div>
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
import Series from "./Series.vue";

export default {
    name: 'Main',
    components: {
        Series,
    },
    data() {
        return {
            series: [
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                "price": "$19.99",
                "series": "Action Comics",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                "price": "$3.99",
                "series": "American Vampire 1976",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                "price": "$16.99",
                "series": "Aquaman",
                "type": "graphic novel"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                "price": "$2.99",
                "series": "Batgirl",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                "price": "$3.99",
                "series": "Batman",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                "price": "$2.99",
                "series": "Batman Beyond",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                "price": "$3.99",
                "series": "Batman/Superman",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                "price": "$4.99",
                "series": "Batman/Superman Annual",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                "price": "$5.99",
                "series": "Batman: The Joker War Zone",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                "price": "$6.99",
                "series": "Batman: Three Jokers",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                "price": "$4.99",
                "series": "Batman: White Knight Presents: Harley Quinn",
                "type": "comic book"
            },
            {
                "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                "price": "$16.99",
                "series": "Catwoman",
                "type": "graphic novel"
            }
        ],
        };
    },

};
</script>

<style lang="scss" scoped>
    main {

        .jumbo {
            background-image: url('../assets/img/jumbotron.jpg');
            height: 400px;
        }
        .container-series {
            background-color: #1C1C1C;
            width: 100%;
            // height: 400px;

            .container {
                display: flex;
                position: relative;
                flex-wrap: wrap;
                padding-top: 2em;

                h2 {
                    background-color: #0282F9;
                    color: #FFFFFF;
                    position: absolute;
                    left: 0;
                    top: -22px;
                    padding: 0.3em 1em;
                }
            }
            div {
                text-align: center;
                padding-top: 0.6em;
                padding-bottom: 1em;

                a {
                    text-decoration: none;
                    background-color: #0282F9;
                    color: #FFFFFF;
                    text-align: center;
                    padding: 0.4em 2em;
                }       
            }
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
                            font-size: 0.9em;
                            text-transform: uppercase;

                        }
                    }
                }
            }
        }
    }
</style>