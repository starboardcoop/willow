<script>
    import Column from "$lib/Column.svelte";
    import Row from "$lib/Row.svelte";
    import Button from "$lib/Button.svelte";
    import Code from "$lib/Code.svelte";
    import Input from "$lib/Input.svelte";
</script>

<h1>Documentation</h1>
<Column>
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
    <Column>
        <h2>Input</h2>
        <Column>
            <Row align="between">
                <h3>Text Input</h3>
                <Input />
            </Row>
            <Code source='<Input />' />
        </Column>
        <Column>
            <Row align="between">
                <h3>Adding a label</h3>
                <Input label="Username" />
            </Row>
            <Code source='<Input label="Username" />' />
        </Column>
        <Column>
            <Row align="between">
                <h3>Adding a placeholder</h3>
                <Input label="Username" placeholder="jsmith" />
            </Row>
            <Code source='<Input label="Username" placeholder="jsmith" />' />
        </Column>
        <Column>
            <Row align="between">
                <h3>Password Input</h3>
                <Input type="password" label="Password" placeholder="Pa$$word" />
            </Row>
            <Code source='<Input type="password" label="Password" placeholder="Pa$$word" />' />
        </Column>
    </Column>
</Column>