<script>
    export let id;
    export let type = "text";
    export let label;
    export let placeholder;
</script>

<div class="flex flex-col gap-2">
    {#if label}
        <label for={id} class="pl-1 text-gray-500 text-sm">{label}</label>
    {/if}
    <input {id} {type} {placeholder} class="bg-gray-100 px-4 py-2 rounded outline-none hover:ring-2 hover:ring-gray-200 focus:ring-2 focus:ring-gray-300" />
</div>