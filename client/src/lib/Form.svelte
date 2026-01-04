<script>
  import Button from './Button.svelte';

  const handleSubmit = () => {
    let lastUser = document.getElementById("username").value;
    console.log("Last Username is " + lastUser);
	// pass above to server
  }
</script>

<form on:submit|preventDefault={handleSubmit}>
  <div class="form-field">
	<input type="text" id="username" spellcheck="false" maxlength=256 placeholder="last.fm username" autofocus="true" autocomplete="off">
  </div>
  <Button>submit</Button>
</form>


<style>
  form {
    display: flex;
	flex-direction: row;
	gap: 12px;
	height: content;
  }
  
  .form-field {
	border-color: red;
  	color: white;
    margin: 8px;
	width: auto;
	height: auto;
  }

  input {
    width: 100%;
	height: 105%;
	border-radius: 2px;
	outline: auto;
  }
</style>
