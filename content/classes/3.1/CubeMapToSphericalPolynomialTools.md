---
TAGS:
---
## Description

class [CubeMapToSphericalPolynomialTools](/classes/3.1/CubeMapToSphericalPolynomialTools)

Helper class dealing with the extraction of spherical polynomial dataArray

from a cube map.

## Methods

### static ConvertCubeMapTextureToSphericalPolynomial(texture) &rarr; [SphericalPolynomial](/classes/3.1/SphericalPolynomial)

Converts a texture to the according Spherical Polynomial data.

This extracts the first 3 orders only as they are the only one used in the lighting.

         * @param texture The texture to extract the information from.

@return The Spherical Polynomial data.

#### Parameters
 | Name | Type | Description
---|---|---|---
 | texture | [BaseTexture](/classes/3.1/BaseTexture) |  The texture to extract the information from.

### static ConvertCubeMapToSphericalPolynomial(cubeInfo) &rarr; [SphericalPolynomial](/classes/3.1/SphericalPolynomial)

Converts a cubemap to the according Spherical Polynomial data.

This extracts the first 3 orders only as they are the only one used in the lighting.

         * @param cubeInfo The Cube map to extract the information from.

@return The Spherical Polynomial data.

#### Parameters
 | Name | Type | Description
---|---|---|---
 | cubeInfo | CubeMapInfo |  The Cube map to extract the information from.

