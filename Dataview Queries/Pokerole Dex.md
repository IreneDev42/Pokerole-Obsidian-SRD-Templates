```dataview
TABLE
Image AS "Image"
FROM #PokeroleSRD/Pokedex
SORT number ASC
WHERE icontains(file.path, "v2.0")
```