<script>
    import Button from "./Button.svelte";
import Input from "./Input.svelte";
    export let title = ''
    export let richText = ''
</script>

<div class="container">
    <h2> { title } </h2>
    <p> { richText } </p>
    <div>
        <Input inputType="important" />
        <Button  textButton="Sign Up" buttonType="danger"/>
    </div>
</div>


<style>
    .container{
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    h2{
        max-width: 400px;
        margin-bottom: 10px;
    }
    p{
        margin-top: 0;
        max-width: 500px;
    }
</style>