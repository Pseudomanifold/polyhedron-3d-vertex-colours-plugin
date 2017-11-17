# An Inkscape plugin for rendering 3D polyhedra with vertex colours

This plugin for the great [Inkscape vector graphics
program](https://inkscape.org) permits rendering 3D
polyhedra&nbsp;(meshes) in [Wavefront OBJ
format](https://en.wikipedia.org/wiki/Wavefront_.obj_file). It is based
on a [similar
plugin](https://gitlab.com/inkscape/inkscape/blob/master/share/extensions/polyhedron_3d.py)
but offers the possibility to use *vertex colours* that are included in
the mesh. This makes the plugin suitable when additional information
such as vertex quality or
[curvature](https://en.wikipedia.org/wiki/Curvature) have to be
visualized.

# Usage

Call the plugin from the *Extensions* menu in Inkscape. A dialog should
pop up that permits you to enter information about the mesh:

<p align="center">

![Main dialog window of the plugin](/Screenshots/Dialog.png?raw=true "Main dialog window of the plugin")

</p>

You can set different viewing options, such as the camera position,
including some transformations, and other styles as well&mdash;these are
taken as-is from the original plugin. It may be useful to experiment
with different settings for the stroke width of the input mesh, in
particular when mesh scales are small.

This is how the example data files should look like:

<p align="center">

![A torus](/Screenshots/Torus.png?raw=true "A torus")

</p>

<p align="center">

![Winged Victory](/Screenshots/Winged_Victory.png?raw=true "Winged Victory")

</p>

# Dependencies

- `numpy`
- `python-lxml`
