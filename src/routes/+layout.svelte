<script>
      import "../app.css";
      import Beach from "./beach.svelte";
</script>
<div class="bg-[#3D4A66] h-full">
    <nav class="flex justify-between h-14 w-full bg-gray-900">
        <div class="pl-2 my-1">
            <a href="/" class=" inline-flex items-center justify-center h-12 px-6 font-medium tracking-wide text-white transition duration-200 bg-gray-900 rounded-lg hover:bg-gray-800 focus:shadow-outline focus:outline-none">
                Home
            </a>
        </div>
        <Beach class="absolute" height="5px" width="5px"/>
        <div class="flex gap-5 mr-4 my-1">
            <a href="/activities" class=" inline-flex items-center justify-center h-12 px-6 font-medium tracking-wide text-white transition duration-200 bg-gray-900 rounded-lg hover:bg-gray-800 focus:shadow-outline focus:outline-none">
                Activities
            </a>
            <a href="/lodging" class=" inline-flex items-center justify-center h-12 px-6 font-medium tracking-wide text-white transition duration-200 bg-gray-900 rounded-lg hover:bg-gray-800 focus:shadow-outline focus:outline-none">
                Lodging
            </a>
            <a href="/faq" class=" inline-flex items-center justify-center h-12 px-6 font-medium tracking-wide text-white transition duration-200 bg-gray-900 rounded-lg hover:bg-gray-800 focus:shadow-outline focus:outline-none">
                FAQ
            </a>
            <a href="/contact" class=" inline-flex items-center justify-center h-12 px-6 font-medium tracking-wide text-white transition duration-200 bg-gray-900 rounded-lg hover:bg-gray-800 focus:shadow-outline focus:outline-none">
                Contact
            </a>
        </div>
    </nav>
    <div class="bg-[#3d4a66] h-full">
        <slot />
    </div>
    <div>
        <footer class="bg-gray-900 text-white text-center text-xs p-3 absolute w-full">
            <h1>&copy; Tahiti 2023</h1>
            <a href="/activities" class="text-white hover:text-gray-400 ml-2">Activities</a>
            <a href="/lodging" class="text-white hover:text-gray-400 ml-2">Lodging</a>
            <a href="/faq" class="text-white hover:text-gray-400 ml-2">FAQ</a>
            <a href="/contact" class="text-white hover:text-gray-400 ml-2">Contact</a>
        </footer>
    </div>
</div>
