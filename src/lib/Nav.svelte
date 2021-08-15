<script>
    import Container from "$lib/Container.svelte";
    import Grid from "$lib/Grid.svelte";
    import Row from "$lib/Row.svelte";
    import Button from "$lib/Button.svelte";

    export let title;
    export let links = [];
</script>

<nav class="w-full">
    <Container>
        <Grid>
            {#if title}
                <Row>
                    <Button type="ghost"><a href="/">{title}</a></Button>
                </Row>
            {/if}
            <Row align="right">
                {#each links as link}
                    <Button type="ghost"><a href={link.href}>{link.label}</a></Button>
                {/each}
            </Row>
        </Grid>
    </Container>
</nav>