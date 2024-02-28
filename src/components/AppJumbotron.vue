<script>

import AppTitle from './AppTitle.vue';

export default {
    name: 'AppJumbotron',
    components: { AppTitle }
}

</script>

<template>
    <div id="jumbotron">
        <div class="text">
            <AppTitle></AppTitle>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptas minus cum, alias ipsa, impedit ducimus,
                repellendus ipsum nostrum dolorem aut ad quod velit perferendis nam qui aliquam voluptatibus aperiam ea?</p>
        </div>
        <div class="img">
            <img src="https://picsum.photos/300/300" alt="">
        </div>
    </div>
</template>

<style>
#jumbotron {
    display: flex;
    gap: 100px;
}

#jumbotron .text {
    text-align: start;
}

#jumbotron img {
    border-radius: 20px;
}

@media screen and (max-width: 768px) {
    #jumbotron {
        flex-direction: column;
    }
}
</style>