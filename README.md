# CarouselMenu
Plugin to create navigation menus with carousel effect

Install
=======
Insert the following source code files in your site.
```html
<script src="js/carousel-menu.js"></script>
<link href="css/carousel-menu.css" rel="stylesheet">
```

How to use
==========
Suppose the following example of navigation menu:
```html
<nav role="navigation" class="navbar">
	<div class="navbar-header">
		<button data-target=".horizontal-menu" data-toggle="collapse" class="navbar-toggle collapsed" type="button">
			<span class="sr-only">Desplegar navegación</span>
			<span class="icon-bar"></span>
			<span class="icon-bar"></span>
			<span class="icon-bar"></span>
		</button>
	</div>

	<div class="collapse navbar-collapse horizontal-menu">
		<ul class="nav navbar-nav">
			<li class="active"><a href="#">Home</a></li>
			<li><a href="#">Link #1</a></li>
			<li><a href="#submenu">Link #2</a></li>
		</ul>
		<ul class="nav navbar-nav">
			<li class="dropdown">
				<a href="#" class="dropdown-toggle" data-toggle="dropdown">Dropdown #1 <b class="caret"></b></a>
				<ul class="dropdown-menu">
					<li><a href="#">Item #1</a></li>
					<li><a href="#">Item #2</a></li>
					<li><a href="#">Item #3</a></li>
				</ul>
			</li>
			<li><a href="#submenu">Link #3</a></li>
			<li><a href="#submenu">Link #4</a></li>
		</ul>
	</div>
</nav>

Basic Use
---------
<script>
	$(function() {
		$('nav').carouselMenu();
	});
</script>

Customized Use
--------------
<script>
	$(function() {
		$('nav').carouselMenu({nextId: "carousel-menu-next", nextClass: "button right", prevId: "carousel-menu-prev", prevClass: "button left", height: '50px', hoverEffect: true});
	});
</script>

Options
-------
__nextId__: Indicates the ID to the "next button" or show the options from the right (followings).
__prevId__: Indicates the ID to the "previous button" or show the options from the left.
__nextClass__: Indicates the CSS class to add into the "next" element.
__prevClass__: Indicates the CSS class to add into the "previous" element.
__hoverEffect__: Indicates if the hover effect must be enabled or not.

