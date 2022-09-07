<script>
import Card from "./lib/Card.svelte";
import Input from "./lib/Input.svelte";
import Menu from "./lib/Menu.svelte";
const menuItems = ["Item1", "Item2", "Item3"];
import Button from './lib/Button.svelte';
import Alert from './lib/Alert.svelte';
import Newsletter from './lib/Newsletter.svelte';
import Counter from "./lib/Counter.svelte";
     
</script>

<Card username="John" 
      imageURL="https://randomuser.me/api/portraits/thumb/men/75.jpg"
      profileURl="https://randomuser.me/api" />

<Input inputType="primary" placeholder="Primary"/>
<Menu {menuItems} />

<Button buttonType="danger" textButton="click"/>
<Alert />
<Alert alertType="archived" status="archived"/>
<Alert alertType="deleted" status="deleted"/>
<Alert alertType="updated" status="upadate"/>
<Newsletter  
title="Lorem, ipsum dolor sit amet consectetur adipisicing elit" 
richText="Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quae dolor officia blanditiis repellat in, 
vero, aperiam porro ipsum laboriosam consequuntur exercitationem incidunt tempora nisi?"/>
<Counter/>
      
      




