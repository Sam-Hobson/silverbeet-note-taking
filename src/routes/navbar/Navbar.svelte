
<script>
    import "../../app.css";
</script>


<nav class="h-14 w-full fixed top-4 flex flex-nowrap justify-center">
    <span class="h-full w-11/12 rounded-3xl flex flex-row overflow-hidden bg-[rgba(200,200,200,0.2)] backdrop-blur">

        <span class="flex justify-start items-center w-full h-full">

            <label for="voice-search" class="sr-only">Search</label>
            <span class="flex relative left-5 w-48 xl:w-80 h-3/5 rounded-3xl pearl-gradient-light shadow justify-center align-middle overflow-hidden">

                <input type="text" class="w-full h-full px-2 outline-none bg-transparent" placeholder="Search for your notes..." required>
                <svg class="w-4 h-full me-3" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 20 20">
                    <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m19 19-4-4m0-7A7 7 0 1 1 1 8a7 7 0 0 1 14 0Z"/>
                </svg>

            </span>

            <span class="w-5"></span>

        </span>

        <span class="hidden sm:flex justify-center items-center whitespace-nowrap w-auto h-full fancy-font text-3xl px-4">
            <a href="/">
            Silverbeet notes
            </a>
        </span>

        <span class="flex justify-end items-center w-full h-full">

            <span class="navbar-menu-option-right hidden xl:block">
                <a href="#target">
                About
                </a>
            </span>

            <span class="navbar-menu-option-right hidden xl:block">
                <a href="#target">
                Features
                </a>
            </span>

            <span class="navbar-menu-option-right hidden xl:block">
                <a href="https://github.com/Sam-Hobson/silverbeet-note-taking/tree/master" target="_blank">
                Source code
                </a>
            </span>

            <span class="w-5"></span>

            <button class="relative right-5 w-48 h-3/5 rounded-3xl pearl-gradient-light shadow opacity-85 hover:opacity-100 transition-all fancy-font text-2xl">
                New note
            </button>

        </span>

    </span>
</nav>


<style>
    .navbar-menu-option-right {
        @apply pr-16 w-auto font-sans text-lg text-gray-700 whitespace-nowrap
    }
</style>
