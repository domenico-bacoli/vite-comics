<script>

export default {
    data() {
        return {

        }
    }
}

</script>


<template>
    <div class="jumbo">

        <div class="container-centered">
            <h3>Content Goes here</h3>
        </div>

    </div>
</template>



<style lang="scss" scoped>
.jumbo {
    display: flex;
    align-items: center;
    background-color: black;
    height: 100px;
    width: 100%;

    .container-centered {
        display: flex;
        align-items: center;
        width: 100%;
    }

    h3 {
        color: white;
    }
}
</style>