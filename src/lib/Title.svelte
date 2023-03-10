<script lang="ts">
    export let fName: String;
    export let lName: String;
    export let description: String;

    $: name = fName + " " + lName;
</script>

    <h1>{name.toLowerCase()}</h1>
    <subtitle>{description.toLowerCase()}</subtitle>

<style>
h1 {
    padding: 5px;
    margin: 5px;
    font-size: 18pt;
    text-align: center;
}
subtitle {
    padding: 5px;
    margin: 5px;
    font-size: 10pt
}
</style>
