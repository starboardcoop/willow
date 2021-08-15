<script>
    import "../app.postcss";
    import Nav from "$lib/Nav.svelte";
    import Main from "$lib/Main.svelte";

    const links = [
        {
            label: "Home",
            href: "/"
        },
        {
            label: "Docs",
            href: "/docs"
        }
    ];
</script>

<Nav title="Willow" {links} />

<Main>
    <slot></slot>
</Main>