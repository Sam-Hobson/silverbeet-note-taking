<script>

    import * as left from './banner-left.png';
    import * as right from './banner-right.png';

</script>


<div class="w-screen h-108 flex flex-row">

    <img src={left.default} class="hidden sm:block w-auto h-full" alt="Decritive plants" />

    <div class="flex w-full h-full banner-background">
        <span class="flex h-full w-full justify-center items-center fancy-font text-6xl text-center xl:text-left">
        Welcome to the<br> Silverbeet notes app...
        </span>

        <span class="hidden xl:flex h-full w-full justify-center items-center text-4xl font-mono leading-relaxed">
        So far you've<br>created _ notes,<br>with _ total words.
        </span>
    </div>

    <img src={right.default} class="hidden sm:block w-auto h-full" alt="Decritive plants" />

</div>


<style>

    .h-108 {
        height: 27rem;
    }

    .banner-background {
        background-color: #ffeae1;
    }

    .fancy-font {
        font-family: 'Parisienne', cursive;
    }

</style>
