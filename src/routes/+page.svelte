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

        <div class="flex flex-col h-full w-auto justify-center items-center">

            <!-- <span class="text-mega-plus font-light pearl-gradient-dark-text leading-none"> -->
            <!-- + -->
            <!-- </span> -->

            <span class="font-mono text-2xl text-gray-800">
            Create your first note by clicking the
            </span>
            <span class="fancy-font text-5xl leading-loose pearl-gradient-dark-text">
            New note
            </span>
            <span class="font-mono text-2xl text-gray-800">
            button
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
        @apply pearl-gradient-dark_
    }

    :global(.pearl-gradient-light) {
        @apply pearl-gradient-light_
     }

     :global(.pearl-gradient-light-text) {
         @apply pearl-gradient-light_ text-transparent;
         background-clip: text;
     }

     :global(.pearl-gradient-dark-text) {
         @apply pearl-gradient-dark_ text-transparent;
         background-clip: text;
     }



    .pearl-gradient-dark_ {
        background: rgb(71,102,255);
        background: linear-gradient(90deg, rgba(71,102,255,1) 0%, rgba(121,206,255,1) 55%, rgba(249,124,255,1) 100%);
    }

     .pearl-gradient-light_ {
         background: rgb(231,235,255);
         background: linear-gradient(90deg, rgba(231,235,255,1) 0%, rgba(228,255,255,1) 44%, rgba(254,231,255,1) 100%);
     }

    .text-mega-plus {
        font-size: 12rem;
    }

</style>
