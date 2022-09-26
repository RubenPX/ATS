<div class="side-header">
	<ul class="side-header-menu">
		<li class="active"><i class="fa fa-copy" /></li>
		<li><i class="fa fa-search" /></li>
		<li><i class="fa fa-share-alt" /></li>
		<li><i class="fa fa-play" /></li>
		<li><i class="fa fa-th-large" /></li>
	</ul>
	<ul class="side-header-botton-menu">
		<li><i class="fa fa-user-circle" /></li>
		<li><i class="fa fa-cog" /></li>
	</ul>
</div>

<style>
	.side-header {
		background: #333;
		position: absolute;
		top: 30px;
		left: 0;
		width: 47px;
		height: calc(100vh - 30px);
	}

	.bottom-header {
		position: absolute;
		bottom: 0;
		left: 0;
		width: 100%;
		height: 20px;
		background: #007acc;
		padding: 0px 10px;
	}

	.side-header li:after {
		content: '';
		position: absolute;
		top: 0;
		left: 0;
		width: 0;
		height: 100%;
		background: #fff;
		transition: all 0.3s linear;
		opacity: 0;
	}

	.side-header li i {
		line-height: 47px !important;
		color: #ccc;
		cursor: pointer;
		font-size: 20px;
	}

	.side-header li {
		text-align: center;
		height: 44px;
		position: relative;
	}
	.side-header li:hover:after {
		width: 2px;
		opacity: 1;
	}

	.side-header li.active:after {
		width: 2px;
		opacity: 1;
	}

	.side-header .active i {
		color: #fff;
	}
	ul.side-header-botton-menu {
		position: absolute;
		width: 100%;
		bottom: 0;
	}
</style>
