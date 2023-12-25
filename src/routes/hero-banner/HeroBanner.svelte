<script>

    import * as left from './banner-left.png';
    import * as right from './banner-right.png';

</script>

<!-- Banner colour: #ffeae1 -->

<div class="w-screen h-108 flex flex-row">

    <img src={left.default} class="w-auto h-full" />

    <div class="w-full h-full banner-background"></div>

    <img src={right.default} class="w-auto h-full" />

</div>


<style>

    .h-108 {
        height: 27rem;
    }

    .banner-background {
        background-color: #ffeae1;
    }

</style>
