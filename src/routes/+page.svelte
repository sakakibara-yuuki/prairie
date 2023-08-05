<script>
    import { LinuxAlt } from "carbon-icons-svelte";

    let cards = [{
        day: "Mar 10, 2023",
        title: "Accessibility tools for designers and developers",
        content: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora expedita dicta totam aspernatur doloremque. Excepturi iste iusto eos enim reprehenderit nisi, accusamus delectus nihil quis facere in modi ratione libero!",
        name: "FugaFuga"
        },{
            day: "Mar 10, 2023",
        title: "Accessibility tools for designers and developers",
        content: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora expedita dicta totam aspernatur doloremque. Excepturi iste iusto eos enim reprehenderit nisi, accusamus delectus nihil quis facere in modi ratione libero!",
        name: "FugaFuga"
        },{
            day: "Mar 10, 2023",
        title: "Accessibility tools for designers and developers",
        content: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora expedita dicta totam aspernatur doloremque. Excepturi iste iusto eos enim reprehenderit nisi, accusamus delectus nihil quis facere in modi ratione libero!",
        name: "FugaFuga"
        },{
            day: "Mar 10, 2023",
        title: "Accessibility tools for designers and developers",
        content: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Tempora expedita dicta totam aspernatur doloremque. Excepturi iste iusto eos enim reprehenderit nisi, accusamus delectus nihil quis facere in modi ratione libero!",
        name: "FugaFuga"
        }]
</script>

<!-- write -->
<div class="hidden sm:flex mx-auto bg-gray-800">
    <div><LinuxAlt size={32} class="bg-white rounded"/></div>
    <div class="w-full">
        <div> bar everyone </div>
        <input type="text" placeholder="What is happening?!" class="block mt-2 w-full h-16 placeholder-gray-400/70 dark:placeholder-gray-500 rounded-lg border border-gray-200 bg-white px-5 py-2.5 text-gray-700 focus:border-blue-400 focus:outline-none focus:ring focus:ring-blue-300 focus:ring-opacity-40 dark:border-gray-600 dark:bg-gray-900 dark:text-gray-300 dark:focus:border-blue-300" />
        <div>evryon can replay</div>
        <div class="flex">icons and post button</div>
    </div>
</div>

{#each cards as card}
<div class="max-w-2xl px-8 py-4 bg-white rounded-lg shadow-md dark:bg-gray-800">
    <div class="flex items-center justify-between">
        <span class="text-sm font-light text-gray-600 dark:text-gray-400">{card.day}</span>
    </div>

    <div class="mt-2">
        <a href="#" class="text-xl font-bold text-gray-700 dark:text-white hover:text-gray-600 dark:hover:text-gray-200 hover:underline" tabindex="0" role="link">{card.title}</a>
        <p class="mt-2 text-gray-600 dark:text-gray-300">{card.content}</p>
    </div>

    <div class="flex items-center justify-between mt-4">
        <a href="#" class="text-blue-600 dark:text-blue-400 hover:underline" tabindex="0" role="link">Read more</a>

        <div class="flex items-center">
            <img class="hidden object-cover w-10 h-10 mx-4 rounded-full sm:block" src="https://images.unsplash.com/photo-1502980426475-b83966705988?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=40&q=80" alt="avatar">
            <a class="font-bold text-gray-700 cursor-pointer dark:text-gray-200" tabindex="0" role="link">{card.name}</a>
        </div>
    </div>
</div>
{/each}