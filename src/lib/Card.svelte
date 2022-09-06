<script>
export let profileURl;
export let imageURL;
export let username;

</script>

<div class="card-container">
    <div class="card">
        <figure>
            <img src="{imageURL}" alt="random-user">
            <figcaption>{username}</figcaption>
        </figure>

    <button>
        <a href="{profileURl}" target="_blank">Profile</a>
    </button>
</div>
</div>

<style>
    .card-container {
        border: 1px solid rgb(56, 56, 56);
        max-width: 20em;
        background-color: rgba(211, 211, 211, 0.652);
    }
    .card {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
    }
    figure {
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    img {
        border-radius: 25%;
    }
    button {
        width: auto;
        height: 3em;
        margin: 1em;
    }
</style>