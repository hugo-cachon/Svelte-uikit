<script>
export let textButton = 'Click me !!';
export let buttonType = 'primary'
  
</script>
<style>
button {
  border-radius: 8px;
  border: 1px solid transparent;
  padding: 0.6em 1.2em;
  font-size: 1em;
  font-weight: 500;
  font-family: inherit;
  cursor: pointer;
  transition: border-color 0.25s;
}

.primary {
  background-color: #249fe7;
  color: white;
}
.danger {
  background-color: #ff0000;
  color: white;
}
.important {
  background-color: #ff6600;
  color: white;
}
button:hover {
  border-color: #FFF;
}


</style>

<button class={buttonType}> { textButton } </button>

