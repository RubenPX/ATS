<script>
	import SideHeader from "./SideHeader.svelte";
</script>

<div class="header">
	<div class="logo">
		<img src="./favicon.png" alt="" />
	</div>
	<ul class="header-menu">
		<li class="header-menu-link">File</li>
		<li class="header-menu-link">Edit</li>
		<li class="header-menu-link">Selection</li>
		<li class="header-menu-link">View</li>
		<li class="header-menu-link">Go</li>
		<li class="header-menu-link">Run</li>
		<li class="header-menu-link">Terminal</li>
		<li class="header-menu-link">Help</li>
	</ul>
	<div class="header-app-icons">
		<ul>
			<li><i class="fa fa-window-minimize" /></li>
			<li><i class="fa fa-window-restore" /></li>
			<li><i class="fa fa-times" /></li>
		</ul>
	</div>
</div>

<SideHeader />

<style>
	.header {
		background: #3c3c3c;
		padding: 5px;
		display: flex;
		align-items: center;
		position: relative;
		max-height: 30px;
	}

	.logo {
		display: inline-block;
        padding: 0 10px;
	}

	ul.header-menu {
		display: inline-block;
		margin-left: 15px;
	}

	ul.header-menu li.header-menu-link {
		display: inline-block;
		color: #cccccc;
		font-weight: 300;
		font-size: 12px;
		margin-right: 10px;
	}

	.logo img {
		width: 17px;
	}

	.header-app-icons {
		position: absolute;
		right: 0;
	}

	.header:after {
		content: '';
		clear: both;
	}

	.header-app-icons li {
		display: inline-block;
		margin: 0 9px;
		color: #ccc;
	}
</style>
