<script>
    import Column from "$lib/Column.svelte";
    import Row from "$lib/Row.svelte";
    import Button from "$lib/Button.svelte";
    import Code from "$lib/Code.svelte";
</script>

<h1>Documentation</h1>
<Column>
    <h2>Button</h2>
    <Column>
        <Row align="between">
            <h3>Normal Button</h3>
            <Button>Button</Button>
        </Row>
        <p>This is the default Button appearance.</p>
        <Code source='<Button>Button</Button>' />
    </Column>
    <Column>
        <Row align="between">
            <h3>Primary Button</h3>
            <Button type="primary">Button</Button>
        </Row>
        <p>This is the primary Button appearance. Suitable for confirmations that respond to pressing Enter/Return.</p>
        <Code source='<Button type="primary">Button</Button>' />
    </Column>
    <Column>
        <Row align="between">
            <h3>Danger Button</h3>
            <Button type="danger">Button</Button>
        </Row>
        <p>This is the danger Button appearance. Suitable for confirmations that are destructive.</p>
        <Code source='<Button type="danger">Button</Button>' />
    </Column>
    <Column>
        <Row align="between">
            <h3>Ghost Button</h3>
            <Button type="ghost">Button</Button>
        </Row>
        <p>This is the ghost Button appearance. Suitable for cases where the button shouldn't draw attention to itself.</p>
        <Code source='<Button type="ghost">Button</Button>' />
    </Column>
</Column>