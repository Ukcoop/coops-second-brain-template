this is the homepage for your second brain!

# Note inbox
these notes have not been organised yet.
```button
name New Note
type command
action Create new note
color purple
```
```dataview
LIST FROM "3 - Resources/inbox"
```
---
# Task inbox
```dataview
TASK
FROM ""
WHERE !completed AND (contains(text, "#task") OR contains(text, "#canDo"))
```
---
# Areas
```button
name New Area
type note(area template) template
action area template
color purple
folder 2 - Areas
prompt true
```
```dataview
LIST FROM "2 - Areas"
WHERE type = "Area"
```
---
# Other resources
```button
name New Resource
type note(resource template) template
action resource template
color purple
folder 3 - Resources
prompt true
```
```dataview
LIST FROM "3 - Resources"
WHERE type = "Resource" AND area = "none"
```
# ideas
```button
name New Idea
type note(idea template) template
action idea template
color purple
folder 3 - Resources/ideas
prompt true
```
```dataview
LIST FROM "3 - Resources/ideas"
WHERE type = "Idea"
```