<script>
    export let align = "left";
    export let inset;

    const justify = () => {
        switch (align) {
            case "between":
                return "justify-between";
            case "right":
                return "justify-end";
            case "left":
            default:
                return "justify-start";
        }
    }
</script>

<div class="flex flex-row gap-4 items-center {justify()}" class:inset>
    <slot></slot>
</div>

<style>
    .inset {
        @apply p-4;
    }
</style>