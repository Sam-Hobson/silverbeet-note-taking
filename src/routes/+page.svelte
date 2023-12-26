<script>
    import Navbar from "./navbar/Navbar.svelte";
    import HeroBanner from "./hero-banner/HeroBanner.svelte";

    let numNotes = 0;
    let wordCount = 0;

</script>

<Navbar />
<HeroBanner numNotes={numNotes} wordCount={wordCount} />

{#if numNotes === 0 }

    <div class="flex w-screen h-128 justify-center">

        <div class="flex flex-col h-full w-auto items-center">

            <span class="text-mega-plus font-light pearl-gradient-dark-text">
            +
            </span>

            <span>
            Dog
            </span>

        </div>

    </div>

{:else}
{/if}


<style>
    @import url('https://fonts.googleapis.com/css2?family=Parisienne&display=swap');

    :global(html) {
        background-color: #fff3ed;
    }

    :global(.h-128) {
        @apply h-[32rem]
    }

    :global(.h-108) {
        @apply h-[27rem]
    }

    :global(.fancy-font) {
        font-family: 'Parisienne', cursive;
    }

    :global(.pearl-gradient-dark) {
        background: rgb(132,153,255);
        background: linear-gradient(90deg, rgba(132,153,255,1) 0%, rgba(207,255,255,1) 55%, rgba(251,169,255,1) 100%); }

    :global(.pearl-gradient-light) {
         background: rgb(231,235,255);
         background: linear-gradient(90deg, rgba(231,235,255,1) 0%, rgba(228,255,255,1) 44%, rgba(254,231,255,1) 100%);
     }

     :global(.pearl-gradient-light-text) {
         @apply pearl-gradient-light text-transparent;
         background-clip: text;
     }

     :global(.pearl-gradient-dark-text) {
         @apply pearl-gradient-dark text-transparent;
         background-clip: text;
     }


    .text-mega-plus {
        font-size: 12rem;
    }

</style>
