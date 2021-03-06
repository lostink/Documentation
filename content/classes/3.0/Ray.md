---
ID_PAGE: 25246
PG_TITLE: Ray
PG_VERSION: 2.1
---
## Description

class [Ray](/classes/3.0/Ray)



## Constructor

## new [Ray](/classes/3.0/Ray)(origin, direction, length)

Defines a [Ray](/classes/3.0/Ray)

#### Parameters
 | Name | Type | Description
---|---|---|---
 | origin | [Vector3](/classes/3.0/Vector3) |   The origin point  The origin point  The origin point  The origin point The origin point
 | direction | [Vector3](/classes/3.0/Vector3) |      The initial vector describing the direction of the [Ray](/classes/3.0/Ray)
optional | length | number |      
## Members

### origin : [Vector3](/classes/3.0/Vector3)

The starting point of the [Ray](/classes/3.0/Ray)

### direction : [Vector3](/classes/3.0/Vector3)

The vector describing the direction of the [Ray](/classes/3.0/Ray)

### length : number



## Methods

### intersectsBoxMinMax(minimum, maximum) &rarr; boolean

Tests if the ray intersects with the box defined by minimum and maximum

#### Parameters
 | Name | Type | Description
---|---|---|---
 | minimum | [Vector3](/classes/3.0/Vector3) |      The minimum vector defining the box
 | maximum | [Vector3](/classes/3.0/Vector3) |      The maximum vector defining the box
### intersectsBox(box) &rarr; boolean

Tests if the ray intersects with the given box

#### Parameters
 | Name | Type | Description
---|---|---|---
 | box | [BoundingBox](/classes/3.0/BoundingBox) |      The box to test with

### intersectsSphere(sphere) &rarr; boolean

Tests if the ray intersects with the given [Sphere](/classes/3.0/Sphere)

#### Parameters
 | Name | Type | Description
---|---|---|---
 | sphere | [BoundingSphere](/classes/3.0/BoundingSphere) |      The sphere to test with

### intersectsTriangle(vertex0, vertex1, vertex2) &rarr; [IntersectionInfo](/classes/3.0/IntersectionInfo)

Tests if the ray intersects with the given triangle defined by the three vectors

#### Parameters
 | Name | Type | Description
---|---|---|---
 | vertex0 | [Vector3](/classes/3.0/Vector3) |      The first vector defining the triangle
 | vertex1 | [Vector3](/classes/3.0/Vector3) |      The second vector defining the triangle
 | vertex2 | [Vector3](/classes/3.0/Vector3) |      The third vector defining the triangle
### intersectsPlane(plane) &rarr; number



#### Parameters
 | Name | Type | Description
---|---|---|---
 | plane | [Plane](/classes/3.0/Plane) |   

### intersectsMesh(mesh, fastCheck) &rarr; [PickingInfo](/classes/3.0/PickingInfo)



#### Parameters
 | Name | Type | Description
---|---|---|---
 | mesh | [AbstractMesh](/classes/3.0/AbstractMesh) |  
optional | fastCheck | boolean |  
### intersectsMeshes(meshes, fastCheck, results) &rarr; Array&lt;[PickingInfo](/classes/3.0/PickingInfo)&gt;



#### Parameters
 | Name | Type | Description
---|---|---|---
 | meshes | Array&lt;[AbstractMesh](/classes/3.0/AbstractMesh)&gt; | 
optional | fastCheck | boolean |  
optional | results | Array&lt;[PickingInfo](/classes/3.0/PickingInfo)&gt; | 
### intersectionSegment(sega, segb, threshold) &rarr; number

Intersection test between the ray and a given segment whithin a given tolerance (threshold)

@return the distance from the ray origin to the intersection point if there's intersection, or -1 if there's no intersection

#### Parameters
 | Name | Type | Description
---|---|---|---
 | sega | [Vector3](/classes/3.0/Vector3) |  the first point of the segment to test the intersection against  the first point of the segment to test the intersection against  the first point of the segment to test the intersection against
 | segb | [Vector3](/classes/3.0/Vector3) |  the second point of the segment to test the intersection against  the second point of the segment to test the intersection against  the second point of the segment to test the intersection against
 | threshold | number |  the tolerance margin, if the ray doesn't intersect the segment but is close to the given threshold, the intersection is successful  the tolerance margin, if the ray doesn't intersect the segment but is close to the given threshold, the intersection is successful  the tolerance margin, if the ray doesn't intersect the segment but is close to the given threshold, the intersection is successful
### static CreateNew(x, y, viewportWidth, viewportHeight, world, view, projection) &rarr; [Ray](/classes/3.0/Ray)

Creates new [Ray](/classes/3.0/Ray)

#### Parameters
 | Name | Type | Description
---|---|---|---
 | x | number |      @param x
 | y | number |      @param y
 | viewportWidth | number |      @param viewportWidth
 | viewportHeight | number |      @param viewportHeight
 | world | [Matrix](/classes/3.0/Matrix) |   a matrix to transform the ray to. Default is the identity matrix.  a matrix to transform the ray to. Default is the identity matrix.  a matrix to transform the ray to. Default is the identity matrix.  a matrix to transform the ray to. Default is the identity matrix. a matrix to transform the ray to. Default is the identity matrix.
 | view | [Matrix](/classes/3.0/Matrix) |      @param view
### static CreateNewFromTo(origin, end, world) &rarr; [Ray](/classes/3.0/Ray)

Function will create a new transformed ray starting from origin and ending at the end point. [Ray](/classes/3.0/Ray)'s length will be set, and ray will be

transformed to the given world matrix.

#### Parameters
 | Name | Type | Description
---|---|---|---
 | origin | [Vector3](/classes/3.0/Vector3) |  The origin point  The origin point  The origin point  The origin point  The origin point The origin point
 | end | [Vector3](/classes/3.0/Vector3) |  The end point  The end point  The end point  The end point  The end point The end point
optional | world | [Matrix](/classes/3.0/Matrix) |  a matrix to transform the ray to. Default is the identity matrix.  a matrix to transform the ray to. Default is the identity matrix.  a matrix to transform the ray to. Default is the identity matrix.  a matrix to transform the ray to. Default is the identity matrix.  a matrix to transform the ray to. Default is the identity matrix. a matrix to transform the ray to. Default is the identity matrix.
### static Transform(ray, matrix) &rarr; [Ray](/classes/3.0/Ray)



#### Parameters
 | Name | Type | Description
---|---|---|---
 | ray | [Ray](/classes/3.0/Ray) |      The given ray
 | matrix | [Matrix](/classes/3.0/Matrix) |      The given matrix to apply
### static TransformToRef(ray, matrix, result) &rarr; void



#### Parameters
 | Name | Type | Description
---|---|---|---
 | ray | [Ray](/classes/3.0/Ray) |      The given ray
 | matrix | [Matrix](/classes/3.0/Matrix) |      The given matrix to apply
 | result | [Ray](/classes/3.0/Ray) |  
