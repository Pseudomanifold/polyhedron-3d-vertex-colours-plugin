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

It may be useful to experiment with different settings for the stroke
width of the input mesh, in particular when mesh scales are small.

# Dependencies

- `numpy`
- `python-lxml`
