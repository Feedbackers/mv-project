# Marija Veselinovic Test
A project for Marija to get some guidance. That is all. Carry on.

# Table of Contents
- [Installation](#installation)
- [BEM Class Methodology](#bem-class-methodology)

# Installation
Download to your project directory:

```sh
  git clone git@gitlab.internal.roundglobe.tech:andrija/react-boilerplate.git && cd mv-test npm install
```

After the installation has finished, start the project by running the command:
```sh
  npm start
```

# BEM Class Methodology:
When naming your classes, use the [BEM](http://getbem.com/) methodology.

BEM stands for **Block**, **Element**, **Modifier**.

A brief example of this can be something like:
- **Block** - .app-navigation
- **Element** - .app-navigation__item
- **Modifier** - .app-navigation__item--red

```html
<nav class="app-navigation">
	<ul>
		<li class="app-navigation__item"> Menu Item 1 </li>
		<li class="app-navigation__item"> Menu Item 2 </li>
		<li class="app-navigation__item--red"> Menu Item Red </li>
	</ul>
</nav>
```

The (S)CSS will look something like this
```scss
.app-navigation {
	display: inline-block;

	&__item {
		display: inline-block;

		color: #000;

		&--red {
			color: red;
		}
	}
}
```
