<script>

    import * as left from './banner-left.png';
    import * as right from './banner-right.png';

    export let numNotes = 0;
    export let wordCount = 0;

</script>


<div class="w-screen h-108 flex flex-row">

    <img src={left.default} class="hidden sm:block w-auto h-full" alt="Decritive plants" />

    <div class="flex w-full h-full bg-[#ffeae1]">
        <span class="flex h-full w-full justify-center items-center fancy-font text-6xl text-center xl:text-left">
        Welcome to the<br> Silverbeet notes app...
        </span>

        <span class="hidden xl:flex h-full w-full justify-center items-center text-4xl font-mono leading-relaxed">
            {#if numNotes === 0 }
                Create a new note to<br/>see some statistics here.
            {:else}
                So far you've<br/>created {numNotes} notes,<br/>with {wordCount} total words.
            {/if}
        </span>
    </div>

    <img src={right.default} class="hidden sm:block w-auto h-full" alt="Decritive plants" />

</div>

