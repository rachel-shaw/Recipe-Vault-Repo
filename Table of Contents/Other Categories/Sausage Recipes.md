---
cssclasses:
  - cards
  - cards-cover
  - table-max
  - cards-cols-4
banner: "![[sausagebanner.jpg]]"
banner_y: 0.628
---

# Sausage Recipes

There are `$= dv.pages("#sausage").length` sausage recipes available below:
```dataview
table without id
	embed(link(cover)),
	file.link as Title,
	"**Difficulty:** " + difficulty as Difficulty,
	"**Prep time:** " + prepTime as "Prep Time",
	"**Cook time:** " + cookTime as "Cook Time",
	"**Rating:** " + rating as "Rating",
	"**Calories: **" + calories as "Calories"
FROM #lunchdinner_recipe and #sausage and -"Templates"
SORT file.name ASC
```



```meta-bind-button
label: Back to Main Menu
icon: "book-open-check"
hidden: false
class: navigation-buttons-center
tooltip: ""
id: menu-button
style: primary
actions:
  - type: open
    link: "[[Menu]]"

```
 
