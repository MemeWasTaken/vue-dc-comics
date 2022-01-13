<template>
    <header>
        <div class="container">
            <img src="../assets/img/dc-logo.png" alt="">
            <ul>
                <li> <a href="#"> Characters </a> </li>
                <li> <a href="#" class="active"> Comics </a> </li>
                <li> <a href="#"> Movies </a> </li>
                <li> <a href="#"> Tv </a> </li>
                <li> <a href="#"> Games </a> </li>
                <li> <a href="#"> Collectibles </a> </li>
                <li> <a href="#"> Videos </a> </li>
                <li> <a href="#"> Fans </a> </li>
                <li> <a href="#"> News </a> </li>
                <li> <a href="#"> Shop </a> </li>
               
            </ul>

        </div>

    </header>
</template>

<script>
export default {
    name: 'Header',
}
</script>

<style lang="scss" scoped>
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;

        img {
            width: 85px;
            height: 85px;
            margin-left: 1em;
        }

        ul {
            list-style: none;
            display: flex;
            justify-content: center;
            align-items: center;
            
            li a {
                text-transform: uppercase;
                color: #464646;
                font-weight: bold;
                display: block;
                text-decoration: none;
                padding: 2.5em 0em;
                margin: 0em 1em;
                &:hover,
                &:active,
                &.active {
                    color: #0282F9;
                    border-bottom: 5px solid #0282F9;
                }
            }

        }
    }
</style>