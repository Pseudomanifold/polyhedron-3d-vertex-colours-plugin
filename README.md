# An Inkscape plugin for rendering 3D polyhedra with vertex colours

This plugin for the great [Inkscape vector graphics
program](https://inkscape.org) permits rendering 3D
polyhedra and meshes in [Wavefront OBJ
format](https://en.wikipedia.org/wiki/Wavefront_.obj_file). It is based
on a [similar
plugin](https://gitlab.com/inkscape/inkscape/blob/master/share/extensions/polyhedron_3d.py)
but offers the possibility to use *vertex colours* that are included in
the mesh. This makes the plugin suitable when additional information
such as vertex quality or
[curvature](https://en.wikipedia.org/wiki/Curvature) have to be
visualized.

The plugin was originally developed to obtain publication-quality vector
graphics for my dissertation. Please refer to [this blog
post](http://bastian.rieck.me/blog/posts/2018/3d_polyhedra) for more
details.

# Installation instructions

* Clone this repository
* Create the path `$HOME/.config/inkscape/extensions` if it does not
  already exist
* Close Inkscape
* Copy the files `polyhedron_3d_vertex_colours.py` and `polyhedron_3d_vertex_colours.inx` into this directory
* Reopen Inkscape
* Enjoy your new plugin, which you can find under *Extensions&ndash;Render*

For more information about installing extensions, please refer to the
[official Inkscape wiki](https://inkscape.org/en/gallery/%3Dextension).

# Usage

Call the plugin from the *Extensions* menu in Inkscape. A dialog should
pop up that permits you to enter information about the mesh:

![Main dialog window of the plugin](/Screenshots/Dialog.png?raw=true "Main dialog window of the plugin")

You can set different viewing options, such as the camera position,
including some transformations, and other styles as well&mdash;these are
taken as-is from the original plugin. It may be useful to experiment
with different settings for the stroke width of the input mesh, in
particular when mesh scales are small.

This is how the example data files should look like:

![A torus](/Screenshots/Torus.png?raw=true "A torus")

![Winged Victory](/Screenshots/Winged_Victory.png?raw=true "Winged Victory")

# Dependencies

The plugin is written in Python. Please install the following packages
using your package manager or `pip`, for example.

- `numpy`
- `python-lxml`

# License

Following the license conditions of the original plugin, this plugin
is also licensed under the GPL Version 2. Please see the file
[LICENSE.md](LICENSE.md) for more information.
