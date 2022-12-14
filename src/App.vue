<template>
    <div class="flex flex-col items-center justify-center h-screen">
        <h1 class="text-3xl font-bold m-2">Vuedo (Vue Todo)</h1>
        <button
            type="button"
            class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700 focus:outline-none dark:focus:ring-blue-800"
        >
            Add Todo
        </button>
        <div>
            <a
                href="#"
                class="block max-w-lg p-6 bg-white border border-gray-200 rounded-lg shadow-md hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700"
            >
                <h5
                    class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"
                >
                    Noteworthy technology acquisitions 2021
                </h5>
                <p class="font-normal text-gray-700 dark:text-gray-400">
                    Here are the biggest enterprise technology acquisitions of
                    2021 so far, in reverse chronological order.
                </p>
                <div class="mt-4">
                    <span
                        class="bg-blue-100 text-blue-800 text-xs font-semibold mr-2 px-2.5 py-0.5 rounded dark:bg-blue-200 dark:text-blue-800"
                        >Default</span
                    >
                    <span
                        class="bg-gray-100 text-gray-800 text-xs font-semibold mr-2 px-2.5 py-0.5 rounded dark:bg-gray-700 dark:text-gray-300"
                        >Dark</span
                    >
                </div>
            </a>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            todos: [
                {
                    id: 1,
                    title: "Todo 1",
                    description: "Todo 1 description",
                    category: ["work", "personal"],
                    completed: false,
                },
                {
                    id: 2,
                    title: "Todo 2",
                    description: "Todo 2 description",
                    category: ["work", "personal"],
                    completed: false,
                },
                {
                    id: 3,
                    title: "Todo 3",
                    description: "Todo 3 description",
                    category: ["work", "personal"],
                    completed: false,
                },
                {
                    id: 4,
                    title: "Todo 4",
                    description: "Todo 4 description",
                    category: ["work", "personal"],
                    completed: false,
                },
                {
                    id: 5,
                    title: "Todo 5",
                    description: "Todo 5 description",
                    category: ["work", "personal"],
                    completed: false,
                },
            ],
            categories: ["work", "personal"],
        };
    },
};
</script>
