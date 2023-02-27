<script lang="ts">

import type { PopupSettings } from '@skeletonlabs/skeleton';	
import { popup } from '@skeletonlabs/skeleton';	


let exampleSettings: PopupSettings = {
	// Set the event as: click | hover | hover-click
	event: 'click',
	// Provide a matching 'data-popup' value.
	target: 'examplePopup'
};
			
</script>
<h1>Test</h1>

<div>
	<button class="btn variant-filled" use:popup={exampleSettings}>
		<span>Menu</span>
		<span class="badge bg-white/10 dark:bg-black/10">Tap</span>
	</button>
	<div class="card variant-filled-secondary p-4 w-72 shadow-xl" data-popup="exampleMenu">
		<!-- NOTE: Keep this wrapper, .space-y will affect the arrow -->
		<div class="space-y-4">
			<p class="font-bold">This is a <strong>Menu</strong> example.</p>
			<p>
				Lorem ipsum dolor sit amet consectetur, adipisicing elit. Dicta amet nam hic aspernatur cum porro praesentium. Voluptates
				velit ex ad eius sit! Sit deserunt ex accusamus quod fugit enim in?
			</p>
			<button class="btn variant-filled">Close Me</button>
		</div>
		<!-- Arrow -->
		<div class="arrow variant-filled-secondary" />
	</div>
</div>