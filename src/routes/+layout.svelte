<script>
    import Icon from "$lib/components/Icon.svelte";
    import "../app.css";
</script>

<div class="py-5 flex bg-white">
    <div class="w-[1000px] mx-auto">
        <div class="flex items-center">
            <a class="block text-3xl" href="/">sheber</a>
            <div class="ml-5 py-2 px-5 rounded-full border border-gray-200">
                <input type="text" placeholder="Поиск" />
            </div>
            <div class="ml-auto gap-x-2 flex items-center">
                <div class="flex w-[50px] h-[50px] bg-gray-100 rounded-full">
                    <Icon
                        color="mx-auto my-auto text-[#FE4B4E]"
                        name="like"
                        size="6"
                    />
                </div>
                <div class="flex w-[50px] h-[50px] bg-gray-100 rounded-full">
                    <Icon
                        color="mx-auto my-auto text-black"
                        name="cart"
                        size="6"
                    />
                </div>
                <a
                    class="block rounded-full bg-black text-white py-3 px-7"
                    href="/login"
                >
                    Создать аккаунт
                </a>
            </div>
        </div>
        <slot />
    </div>
</div>
