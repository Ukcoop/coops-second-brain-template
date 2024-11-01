---
type: Area
---
# Overview
A area could be for a part of your life that needs maintained, like finances or house, or like your career (ex. Software development).
# Projects
```button
name New project
type note(project template) template
action project template
color purple
folder 1 - Projects
prompt true
```
```dataview
LIST FROM "1 - projects"
WHERE type = "Project" AND area = this.file.name
```
---
# Resources
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
WHERE type = "Resource" OR type = "Idea" AND area = this.file.name
```