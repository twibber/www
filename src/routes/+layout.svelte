<script>
    import "~/styles/tailwind.css"

    import Navbar from "~/components/Navbar.svelte";
    import Sidebar from "~/components/Sidebar.svelte";

	export let data;
</script>

<div class="font-medium bg-gray-800 text-white">
    <div class="grid grid-cols-8 grid-flow-col min-h-screen max-w-screen-lg mx-auto">
        <Navbar {data}/>
        <main class="col-span-4">
            <slot/>
        </main>
        <Sidebar/>
    </div>
</div>