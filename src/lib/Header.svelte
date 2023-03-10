<script lang="ts">
    import Title from "./Title.svelte";
    export let fName: String;
    export let lName: String;
    export let description: String;
</script>

<div class="header">
    <Title {fName} {lName} {description} />
</div>

<style>
    .header {
        text-align: center;
        flex-direction: column;
    }
</style>
