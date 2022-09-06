<script>
export let inputType;
</script>

<input class={inputType} type="text" required>

<style>
    input[type=text] {
        outline: none;
        padding: 3px 0px 3px 3px;
        margin: 5px 1px 3px 0px;
        border: 1px solid #DDDDDD;
    }
    .primary:focus {
        box-shadow: 0 0 5px rgb(81, 81, 238);
        padding: 3px 0px 3px 3px;
        margin: 5px 1px 3px 0px;
        border: 1px solid rgb(64, 82, 219);
    }
    .important:focus {
        box-shadow: 0 0 5px rgb(242, 153, 57);
        padding: 3px 0px 3px 3px;
        margin: 5px 1px 3px 0px;
        border: 1px solid rgb(230, 97, 9);
    }
    .danger:focus {
        box-shadow: 0 0 5px rgb(219, 48, 48);
        padding: 3px 0px 3px 3px;
        margin: 5px 1px 3px 0px;
        border: 1px solid rgb(188, 26, 26);
    }
</style>