---
aliases:
  - Project Template
Author: Atharva Chavan
Created: 2025-02-22
Updated: 
tags:
  - ProjectPlan
Comments:
---

# Project Template

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
```dataview
TABLE WITHOUT ID 
	link(file.name,file.aliases[0]) as "Note",
	Comments as "Description"
WHERE 
	contains(file.path, this.file.folder) 
	AND file.name != this.file.name
SORT file.aliases[0] ASC
```


## Connections
- [[2025-02-22]] - Daily Note for day this file was created.