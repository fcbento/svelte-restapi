<script>
    
    import Form from "./form.svelte";
    import Table from "./table.svelte";

    export let fields;
    export let endpoint;
    export let colSize;
    export let type;
    export let headers;
    export let body;

</script>

<div class="row">

    <Form {fields} {endpoint} {colSize}/>

    <div class="col">
        <Table {type} {headers} {body} {endpoint} />
    </div>
    
</div>
