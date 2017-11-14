# CSS Color API

## Endpoints:

## Random Color

### `randomcolor`

**GET** _gets a random color_

**Example:** `https://fun-fun-colors.herokuapp.com/randomcolor`


**NOTE** Please use the proper headers. This will work:
`headers: {
	'Accept': 'application/json',
	'Content-Type': 'application/json'
}`

#### Sample Response 

#### Success

	{
		color: 'plum',
		status: 200
	}

#### Fail

	{
		error: 'Error message',
		status: 500
	}

## Color by Name

### `colorcheck`

**GET** _gets a specific color from the list_

**NOTE** Please use the proper headers. This will work:
`headers: {
	'Accept': 'application/json',
	'Content-Type': 'application/json'
}`

This will return a color from the CSS Colors. The list is in alphabetical order. The possible numbers range from **0 to 146**


Params | Value | Description | Valid format example
------ | ---- | ------ | ------
`q` | string | `the color or part of the color to return the index of` | 22


**Example:** `https://fun-fun-colors.herokuapp.com/colorcheck?q=dark` || `https://fun-fun-colors.herokuapp.com/colorcheck?q=darkcyan`


#### Success

	{
		colorIndex: 22,
		status: 200
	}

#### Fail

	{
		error: 'Error message',
		status: 500
	}

## Color by id

### `color/:id`

**GET** _gets a specific color from the list_

**NOTE** Please use the proper headers. This will work:
`headers: {
	'Accept': 'application/json',
	'Content-Type': 'application/json'
}`

This will return a color from the CSS Colors. The list is in alphabetical order. The possible numbers range from **0 to 146**


Params | Value | Description | Valid format example
------ | ---- | ------ | ------
`id` | number | `the id/index of the color to return` | 22


**Example:** `https://fun-fun-colors.herokuapp.com/color/22`


#### Success

	{
		color: 'darkcyan',
		status: 200
	}

#### Fail

	{
		error: 'Error message',
		status: 500
	}



## All Colors

### `allcolors`

**GET** _gets an array of all colors_

**NOTE** Please use the proper headers. This will work:
`headers: {
	'Accept': 'application/json',
	'Content-Type': 'application/json'
}`

This will return an array of all CSS colors. The list is in alphabetical order.



**Example:** `https://fun-fun-colors.herokuapp.com/allcolors`


#### Success

	{
		status: 200,
		color: [
			"aliceblue",
			"antiquewhite",
			"aqua",
			"aquamarine",
			"azure",
			"beige",
			"bisque",
			"black",
			"blanchedalmond",
			"blue",
			"blueviolet",
			"brown",
			"burlywood",
			"cadetblue",
			"chartreuse",
			"chocolate",
			"coral",
			"cornflowerblue",
			"cornsilk",
			"crimson",
			"cyan",
			"darkblue",
			"darkcyan",
			"darkgoldenrod",
			"darkgray",
			"darkgrey",
			"darkgreen",
			"darkkhaki",
			"darkmagenta",
			"darkolivegreen",
			"darkorange",
			"darkorchid",
			"darkred",
			"darksalmon",
			"darkseagreen",
			"darkslateblue",
			"darkslategray",
			"darkslategrey",
			"darkturquoise",
			"darkviolet",
			"deeppink",
			"deepskyblue",
			"dimgray",
			"dimgrey",
			"dodgerblue",
			"firebrick",
			"floralwhite",
			"forestgreen",
			"fuchsia",
			"gainsboro",
			"ghostwhite",
			"gold",
			"goldenrod",
			"gray",
			"grey",
			"green",
			"greenyellow",
			"honeydew",
			"hotpink",
			"indianred",
			"indigo",
			"ivory",
			"khaki",
			"lavender",
			"lavenderblush",
			"lawngreen",
			"lemonchiffon",
			"lightblue",
			"lightcoral",
			"lightcyan",
			"lightgoldenrodyellow",
			"lightgray",
			"lightgrey",
			"lightgreen",
			"lightpink",
			"lightsalmon",
			"lightseagreen",
			"lightskyblue",
			"lightslategray",
			"lightslategrey",
			"lightsteelblue",
			"lightyellow",
			"lime",
			"limegreen",
			"linen",
			"magenta",
			"maroon",
			"mediumaquamarine",
			"mediumblue",
			"mediumorchid",
			"mediumpurple",
			"mediumseagreen",
			"mediumslateblue",
			"mediumspringgreen",
			"mediumturquoise",
			"mediumvioletred",
			"midnightblue",
			"mintcream",
			"mistyrose",
			"moccasin",
			"navajowhite",
			"navy",
			"oldlace",
			"olive",
			"olivedrab",
			"orange",
			"orangered",
			"orchid",
			"palegoldenrod",
			"palegreen",
			"paleturquoise",
			"palevioletred",
			"papayawhip",
			"peachpuff",
			"peru",
			"pink",
			"plum",
			"powderblue",
			"purple",
			"rebeccapurple",
			"red",
			"rosybrown",
			"royalblue",
			"saddlebrown",
			"salmon",
			"sandybrown",
			"seagreen",
			"seashell",
			"sienna",
			"silver",
			"skyblue",
			"slateblue",
			"slategray",
			"slategrey",
			"snow",
			"springgreen",
			"steelblue",
			"tan",
			"teal",
			"thistle",
			"tomato",
			"turquoise",
			"violet",
			"wheat",
			"white",
			"whitesmoke",
			"yellow",
			"yellowgreen"
		]
	}

#### Fail

	{
		error: 'Error message',
		status: 500
	}
