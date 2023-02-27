<script lang="ts">

import type { PopupSettings } from '@skeletonlabs/skeleton';	
import type { popup } from '@skeletonlabs/skeleton';	


let exampleSettings: PopupSettings = {
	// Set the event as: click | hover | hover-click
	event: 'click',
	// Provide a matching 'data-popup' value.
	target: 'examplePopup'
};
			


</script>
<h1>Test</h1>

<button class="btn variant-filled" use:popup={exampleSettings}>
	<span>Menu</span>
	<span class="badge bg-white/10 dark:bg-black/10">Tap</span>
</button>