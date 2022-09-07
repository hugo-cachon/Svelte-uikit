<script>
import Card from "./lib/Card.svelte";
import Input from "./lib/Input.svelte";
import Menu from "./lib/Menu.svelte";
import Details from "./lib/Details.svelte";
const menuItems = ["Item1", "Item2", "Item3"];
let src = "https://dynamic-media-cdn.tripadvisor.com/media/photo-o/1d/b9/99/5c/moraine-lake-photo-taken.jpg?w=1000&h=-1&s=1";
</script>

<Card username="John" 
      imageURL="https://randomuser.me/api/portraits/thumb/men/75.jpg"
      profileURl="https://randomuser.me/api" />

<Input inputType="primary" placeholder="Primary"/>

<Menu {menuItems} />

<Details {src} alt="Moraine Lake" detailsTitle="DetailsTitle" detailsText="DetailsText"/>


      




