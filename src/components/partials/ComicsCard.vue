<template>
    <div class="cardComics">
        
        <img :src="img" :alt="name">
        <h6>{{name}}</h6>

    </div>
</template>

<script>
export default {
    name: "ComicsCard",
    props: {
        "img": String,
        "name": String
    },
}
</script>

<style scoped lang="scss">
    .cardComics{
        width: calc(100% / 6);
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        padding: 10px;
        
       

        img{
            width: 100%;
            aspect-ratio: 1;
            object-fit: cover;
            object-position: top;
        }

        h6{
            color: white;
            font-size: 12px;
            font-weight: 400;
            text-transform: uppercase;
            margin-top: 10px;
        }
    }
</style>