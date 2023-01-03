<template>
    <div class="flex flex-col items-center justify-center">
        <h1 class="text-3xl font-bold m-2">Vuedo (Vue Todo)</h1>
        <button
            type="button"
            class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 mb-2 dark:bg-blue-600 dark:hover:bg-blue-700 focus:outline-none dark:focus:ring-blue-800 mb-8"
        >
            Add Todo
        </button>
        <div class="max-w-lg flex flex-col items-center justify-center">
            <div v-for="todo in todos">
                <div
                    href="#"
                    class="block min-w-[300px] md:min-w-[600px] p-6 bg-white border border-gray-200 rounded-lg shadow-md hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700 mb-6"
                >
                    <h5
                        class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"
                    >
                        {{ todo.title }}
                    </h5>
                    <p class="font-normal text-gray-700 dark:text-gray-400">
                        {{ todo.description }}
                    </p>
                    <div class="mt-4">
                        <span
                            v-for="category in todo.category"
                            class="bg-blue-100 text-blue-800 text-xs font-semibold mr-2 px-2.5 py-0.5 rounded dark:bg-blue-200 dark:text-blue-800"
                            >{{ category }}
                        </span>
                    </div>
                </div>
            </div>
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
                    category: ["work", "personal", "shopping"],
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
            categories: ["work", "personal", "shopping", "others"],
        };
    },
};
</script>
