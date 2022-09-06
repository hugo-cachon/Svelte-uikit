<script>
export let menuItems;
let menuOpen = false;
</script>

<section class="dropdown-menu">
  <button on:click={() => menuOpen = !menuOpen}> Menu </button>
  <ul class="menu-items" class:show={menuOpen}>			
    {#if menuItems.length > 0}
        {#each menuItems as item}
    <li>{item}</li>
        {/each}
    {/if}		
  </ul>	
</section>
	
<style>		
    .dropdown-menu {
        position: relative;
    }
    .menu-items {
        display: none;
        position: absolute;
        margin-top: 0em;
        background-color: rgba(211, 211, 211, 0.652);
        min-width: 230px;
    }	
    li {
        list-style: none;
    }
    .show {
        display: block
    }
</style>