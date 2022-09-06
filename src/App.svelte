<script>
import Card from "./lib/Card.svelte";
import Input from "./lib/Input.svelte";
import Menu from "./lib/Menu.svelte";
const menuItems = ["Item1", "Item2", "Item3"];
</script>

<Card username="John" 
      imageURL="https://randomuser.me/api/portraits/thumb/men/75.jpg"
      profileURl="https://randomuser.me/api" />

<Input inputType="primary" placeholder="Primary"/>

<Menu {menuItems} />



      




