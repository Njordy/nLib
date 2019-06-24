nLib
====

A growing collection of digital assets what might be helpful to a beginning Houdini artist. 
Every tool does a simple operations what is usually very common. 


### Tools

General purpose nodes:
- **Positional Change**: takes original and deformed geometry, and adds a v@pchange with a difference between positions on these geos; contains a visualization option and a mix slider. 
- **Calcualte Curve U**: fastest way to create @curve_u attribute, also can convert from @uv in order to save a little bit of memory.
- **Calcualte Curve Tangent**: better way to calculate tangent — every point points at the next one, and the end point of every curve continues the direction instead of breaking; additional randomization of the end point vectors (on set angle) and @end attribute to easily separate last points on the curve. 
- **Curve Root**: creates @root attribute (or a group "roots") in the very first point of every curve; has an option of leaving only root points.
- **Curve Rotate**: (useful for grass and hair) rotates a curve (by @root point) to a specufied angle with option to add randomization.

Simulational:
- **Positional Change**: takes volume primitives from a smoke simulation, converts to VDBs, merges multiple scalar fields into vector field, deactivates voxels beyound bounaries of @density with option to downsample any of them. 

Hair and Fur:
- **Fur Vusualizer**: colorizes hair randomly, also appliying unified color onth hairs in one clump on top;  has an additional option to color guard hair with different color.
- **Hair Clump Radius Randomize**: just sets a random attribute @clumpsize on guide hair. 
- **Guide Influence Radius**: helps then guides on the skin were planted with different density, so it calculates @influenceradiusscale attribute on order to set in influence individually in order to limit interpolation from destroying fine ditails.  
- **Hair Clump Anisotropy**: takes @anisotropy_dir skin attribute and moves clumped hair in it's direction in order to make it look similarly to wolf's mane.  

### Installation

[Hoduini Documentation](http://www.sidefx.com/docs/houdini/ref/plugins.html)

### Acknowledgement

Hair-related tools are based on algorithms by Alex Sknarin. 
