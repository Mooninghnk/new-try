<script lang="ts">
    let isOpen = false;

    function toggleMenu() {
        isOpen = !isOpen;
    }
    function closeMenu() {
      isOpen = false;
    }
</script>

<nav class="navbar bg-base-100 p-4 flex justify-between items-center">
    <div class="flex-1 flex items-center">
        <a class="btn btn-ghost normal-case text-xl" href="/">Benzcode Tutoring</a>
    </div>
    <div class="flex-none hidden lg:flex gap-4">
        <a class="btn btn-ghost normal-case text-xl" href="/login">Login</a>
        <a class="btn btn-ghost normal-case text-xl" href="/register">Register</a>
        <a class="btn btn-primary normal-case text-xl" href="/trial">Free trial</a>
    </div>
    <div class="lg:hidden">
        <button class="btn btn-ghost" on:click={toggleMenu}>
            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
            </svg>
        </button>
    </div>
    {#if isOpen}
    <div class="fixed inset-0 flex items-center justify-center bg-base-100 bg-opacity-90 z-50">
      <div class="flex flex-col items-center space-y-4 bg-white bg-opacity-30 backdrop-blur-md p-8  glass rounded-lg shadow-lg ">
            <button class="btn btn-ghost" on:click={closeMenu}>
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                </svg>
            </button>
            <a class="btn btn-ghost normal-case text-xl" href="/login">Login</a>
            <a class="btn btn-ghost normal-case text-xl" href="/register">Register</a>
            <a class="btn btn-primary normal-case text-xl" href="/trial">Free trial</a>
        </div>
    </div>

    {/if}
</nav>
