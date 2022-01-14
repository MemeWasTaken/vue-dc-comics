<template>
  <div class="serie">
        <div class="container-img">
            <img :src="img">
        </div>
        <h3> {{ title }} </h3>
  </div>
</template>

<script>
export default {
    name: "Series",
    props: ['img', 'title'],
}
</script>

<style lang="scss">
    .serie {
        flex-basis: calc((100% / 6) - 0.4em);
        margin: 0.2em;
        padding: 1em;
        
        .container-img {
            width: 185px;
            height: 185px;
            overflow: hidden;

            img {
                width: 100%;
            }
        }

        h3 {
            color: #FFFFFF;
            font-size: 0.9em;
            margin-top: 1.5em;
            text-align: start;
        }
    }
</style>