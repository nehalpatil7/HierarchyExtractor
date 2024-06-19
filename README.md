# HierarchyExtractor
JSON object Hierarchy Extractor

## Extract all distinct keys in JSON objects in hierarchical order

### Required packages
1. json
2. anytree
3. os
4. glob

### Function description
|param  : path to JSON file(with .json entension at the end) or directory containing multiple JSON files
|returns: object hierarchy in JSON in graphical format

### Example

```json
{
	"id": "0001",
	"type": "donut",
	"name": "Cake",
	"ppu": 0.55,
	"batters":
		{
			"batter":
				[
					{ "id": "1002", "type": "Chocolate" },
				]
		},
	"topping":
		[
			{ "id": "5005", "type": "Sugar" },
		]
}
```

```bash
Visualizing keys for Users/Desktop/example.json
root
|-- id
|-- type
|-- name
|-- ppu
|-- batters
|   +-- batter
|       |-- id
|       +-- type
+-- topping
    |-- id
    +-- type
```
