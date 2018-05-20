# WorkGrid
Work grid is a basic grid and cell system based on flex box. Very much a work in progress, but it works because it is simple.

## Basics
To use WorkGrid just add the CSS.
```
<link rel="stylesheet" href="work.css" />
```

WorkGrid has a few classes that are helpful
`<div class=“work row”>` is the primary container for a WorkGrid
`<div class="work col">` is a column. Work grid is based on a 12 column layout.
`<div class="work cell">` is a cell. Cells can be stacked inside of columns. Once you use a cell, it is recommended to use a cell in all remaining columns in the row.

## Example
This example produces a three column grid on a single row.
Each cell has a set height to demonstrate how WorkGrid adjusts appropriately.
```
<div class="work row">
	<div class="work col">
		<div class="work cell short">This is 2rem</div>
		<div class="work cell medium">This is 5rem</div>
		<div class="work cell tall">This is 10rem</div>
	</div>
	<div class="work col">
		<div class="work cell">This is auto height</div>
	</div>
	<div class="work col">
		<div class="work cell tall">This is 10rem</div>
			<div class="work cell short">This is 2rem</div>
			<div class="work cell">This is auto heigh</div>
		</div>
	</div>	
```