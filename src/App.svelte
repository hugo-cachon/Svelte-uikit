<script>
import Card from "./lib/Card.svelte";
import Input from "./lib/Input.svelte";
import Menu from "./lib/Menu.svelte";
import Details from "./lib/Details.svelte";
const menuItems = ["Item1", "Item2", "Item3"];
let src = "https://dynamic-media-cdn.tripadvisor.com/media/photo-o/1d/b9/99/5c/moraine-lake-photo-taken.jpg?w=1000&h=-1&s=1";
import Button from './lib/Button.svelte';
import Alert from './lib/Alert.svelte';
import Counter from "./lib/Counter.svelte";
import GridTile from "./lib/GridTile.svelte";
let product = {
    title: 'No product provided',
    src: 'https://img.icons8.com/ios/500/no-image.png',
    cost: '$0',

  };
import Red from './lib/Red.svelte';
import Green from './lib/Green.svelte';

	const options = [
		{ color: 'red',   component: Red },
		{ color: 'green', component: Green },
	];

	let selected = options[0];
     
</script>

<select bind:value={selected}>
	{#each options as option}
		<option value={option}>{option.color}</option>
	{/each}
</select>

{#if selected.color === 'red'}
	<Red/>
{:else if selected.color === 'green'}
	<Green/>
{/if}

<Card username="John" 
      imageURL="https://randomuser.me/api/portraits/thumb/men/75.jpg"
      profileURl="https://randomuser.me/api" />

<Input inputType="primary" placeholder="Primary"/>
<Menu {menuItems} />

<Details {src} alt="Moraine Lake" detailsTitle="DetailsTitle" detailsText="DetailsText"/>


<Button buttonType="danger" textButton="click"/>
<Alert />
<Alert alertType="archived" status="archived"/>
<Alert alertType="deleted" status="deleted"/>
<Alert alertType="updated" status="upadate"/>
<Counter/>
<Counter/>
<GridTile {product} />
