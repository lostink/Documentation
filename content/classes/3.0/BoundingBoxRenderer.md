---
ID_PAGE: 25300
PG_TITLE: BoundingBoxRenderer
PG_VERSION: 2.1
TAGS:
    - Mesh
    - Bounding
---
## Description

class [BoundingBoxRenderer](/classes/3.0/BoundingBoxRenderer)



## Constructor

## new [BoundingBoxRenderer](/classes/3.0/BoundingBoxRenderer)(scene)

Creates a new renderer used to display the bounding box of its render list

#### Parameters
 | Name | Type | Description
---|---|---|---
 | scene | [Scene](/classes/3.0/Scene) |      The scene linked to this [BoundingBoxRenderer](/classes/3.0/BoundingBoxRenderer)

## Members

### frontColor : [Color3](/classes/3.0/Color3)

The front color of the bounding box

### backColor : [Color3](/classes/3.0/Color3)

The back color of the bounding box

### showBackLines : boolean

True if back lines should be displayed, false otherwise

default : true

### renderList : [SmartArray](/classes/3.0/SmartArray)&lt;[BoundingBox](/classes/3.0/BoundingBox)&gt;

This renderer render list

## Methods

### reset() &rarr; void

Reset the render list
### render() &rarr; void

The render function
### dispose() &rarr; void


