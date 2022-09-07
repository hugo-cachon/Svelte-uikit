<script>
export let detailsTitle;
export let detailsText;
export let src;
export let alt;

</script>

<div class="container">
    <div class="details-container">
    <figure>
        <img src={src} alt={alt}>
    </figure>

    <details>
        <summary>{detailsTitle}</summary>
        {detailsText}
    </details>
    </div>
</div>

<style>
.container {
    display: inline-block;
    border: 1px solid #aaa;
    border-radius: 4px;
    padding: .5em .5em 0;
}
.details-container {
    display: flex;
    flex-direction: column;
}

img {
    max-width: 20em;
}

figure {
    margin: 1em 0;
} 


summary {
    font-weight: bold;
    margin: -.5em -.5em 0;
    padding: .5em;
    width: 20em;
}


details[open] summary {
    border-bottom: 1px solid #aaa;
    margin-bottom: .5em;
} 
</style>
