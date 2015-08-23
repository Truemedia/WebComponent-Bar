# Web Component - Bar
A web component spec for bars, for making percentage/fraction based UI such as progress bars

This is an experimental spec as my first attempt at making a web component.

The base element is `<bar></bar>` with 3 variations with specific attribute and styling differences. The content of the element serves as the label.

The main purpose of this repo is to slim down the complexity of bar based UIs, while adding some easy options for doing fancy looking things.

### Variations

- Progress bar, **percentage** attribute and **fraction** attribute with none animated expanding bar
- Health bar, **current-points** (integer) attribute, **min-points** (integer) attribute, **max-points** (integer) attribute with **color-boundaries** attribute for changing bar color based on number range
- Equalizer bar, **units** attribute serving as a label, **value** attribute for current value, **maxed** attribute for maximum value, and clipping attribute for displaying visual warning when maximum value reached or exceeded.


### Examples
##### Progress bar
    <progress-bar percentage="64">Running a process, please wait...</progress-bar>

##### Health bar
	<health-bar current-points="24" min-points="-5" max-points="250" color-boundaries='{"0-50": "#00ff00" }'>Health</health-bar>

##### Equalizer bar
    <equalizer-bar units="db" value="30" maxed="120">Track 1</equalizer-bar>

