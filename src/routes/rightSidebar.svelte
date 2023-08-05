<script>
    let users = [{
        name: 'Arthur Melo',
        id: '@authurmelo',
        icon: "https://images.unsplash.com/photo-1535713875002-d1d0cf377fde?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=880&q=80",
        },{
        name: 'junior REIS',
        id: '@junior',
        icon: "https://images.unsplash.com/photo-1608174386344-80898cec6beb?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=687&q=80", 
        },{
        name: 'Olivia Wathan',
        id: '@oliviawathan',
        icon: "https://images.unsplash.com/photo-1488508872907-592763824245?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1470&q=80",
        },{
        name: 'Mia',
        id: '@mia',
        icon: "https://images.unsplash.com/photo-1499470932971-a90681ce8530?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1470&q=80",
        }
    ]
</script>


<!-- search bar -->
<div class="sticky top-0 z-50">
    <div class="relative mt-2 mb-4">
        <span class="absolute inset-y-0 left-0 flex items-center pl-3">
            <svg class="w-5 h-5 text-gray-400" viewBox="0 0 24 24" fill="none">
                <path d="M21 21L15 15M17 10C17 13.866 13.866 17 10 17C6.13401 17 3 13.866 3 10C3 6.13401 6.13401 3 10 3C13.866 3 17 6.13401 17 10Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"></path>
            </svg>
        </span>
        <input type="text" class="w-full py-2 pl-10 pr-4 text-gray-700 bg-white border rounded-md dark:bg-gray-900 dark:text-gray-300 dark:border-gray-600 focus:border-blue-400 dark:focus:border-blue-300 focus:ring-blue-300 focus:ring-opacity-40 focus:outline-none focus:ring" placeholder="Search" />
    </div>
</div>
<!-- search bar -->
  

<!-- cards 1 -->
<div class="w-full max-w-sm px-4 py-3 bg-white rounded-md shadow-md dark:bg-gray-800">
    <h1 class="mt-2 text-lg font-semibold text-gray-800 dark:text-white">Get Verified</h1>
    <p class="mt-2 text-sm text-gray-600 dark:text-gray-300">Subscribe to unlock new features.</p>
    <button class="bg-blue-500 rounded-md text-white">Get Verified</button>
</div>


<div class="flex flex-col mt-6">
    <div class="inline-block min-w-full align-middle">
        <div class="overflow-hidden border border-gray-200 dark:border-gray-700 md:rounded-lg">
            <table class=" divide-gray-200 dark:divide-gray-700">
                <thead class="bg-gray-50 dark:bg-gray-800">
                    <tr>
                        <th scope="col" class="py-3.5 px-4' text-lg text-left rtl:text-right text-gray-500 dark:text-gray-400">
                            <div>Who to follow</div>
                        </th>
                        <th>
                        </th>
                    </tr>
                </thead>
                <tbody class="bg-white divide-y divide-gray-200 dark:divide-gray-700 dark:bg-gray-900">
                    {#each users as user}
                    <tr>
                        <td class="px-4 py-4 text-sm font-medium text-gray-700 whitespace-nowrap">
                            <div class="inline-flex items-center gap-x-3">
                                <div class="flex items-center gap-x-2">
                                    <img class="object-cover w-10 h-10 rounded-full" src={user.icon} alt="">
                                    <div>
                                        <h2 class="font-medium text-gray-800 dark:text-white ">{user.name}</h2>
                                        <p class="text-sm font-normal text-gray-600 dark:text-gray-400">{user.id}</p>
                                    </div>
                                </div>
                            </div>
                        </td>
                        <td class="px-12 py-4 text-sm font-medium text-gray-700 whitespace-nowrap">
                            <div class="inline-flex items-center px-3 py-1 rounded-full gap-x-2 bg-white">
                                <h2 class="text-sm font-normal text-blue-900">Follow</h2>
                            </div>
                        </td>
                    </tr>
                    {/each}
                </tbody>
            </table>
        </div>
    </div>
</div>