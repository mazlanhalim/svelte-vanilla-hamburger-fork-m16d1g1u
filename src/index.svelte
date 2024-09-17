<script>
	import 'vanilla-hamburger';

	let count = 0;

	function handlePressedChanged(event) {
		if (event.target.pressed) {
			count += 3;
		}
	}
</script>

<style>
	tilt-burger {
		margin: 0 auto;
	}

	output {
		display: block;
		margin-top: 00px;
		font-size: 3rem;
		font-family: 'Open Sans';
		text-align: center;
	}
</style>

<div>
	<tilt-burger on:pressed-changed="{handlePressedChanged}"></tilt-burger>
	<output>{count} clicks</output>
</div>