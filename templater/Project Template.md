---
aliases:
  - <% tp.file.title.slice(1) %>
Author: Atharva Chavan
Created: <% tp.file.creation_date("YYYY-MM-DD") %>
Updated: 
tags:
  - ProjectPlan
Comments:
---

# <%tp.file.title.slice(1)%>

## Overview
_Quick overview, purpose, standards._  

## Goal
_link to goal_

## Done Looks Like
_how do I know I'm done?_

## Branches

## Resources


## Plans
- [ ] What is next?

## Journal
- 


## Files
```sql
TABLE WITHOUT ID 
	link(file.name,file.aliases[0]) as "Note",
	Comments as "Description"
WHERE 
	contains(file.path, this.file.folder) 
	AND file.name != this.file.name
SORT file.aliases[0] ASC
```


## Connections
- [[<% tp.date.now("YYYY-MM-DD") %>]] - Daily Note for day this file was created.