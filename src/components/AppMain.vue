<script>
import AppBluBandSection from './AppBluBandSection.vue';


export default {
    data() {
        return {};
    },
    components: { AppBluBandSection }
}

</script>


<template>
    <div class="main">
        <div class="container-centered">
            <h3>Content Goes here</h3>
        </div>
    </div>
    <AppBluBandSection></AppBluBandSection>
</template>



<style lang="scss" scoped>
.main {
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