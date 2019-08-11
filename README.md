# Xampane

Xamarin.Forms **Layouts** library.

<img src="images/xampane.png" Width="150" />

### CircularLayout

The CircularLayout is a simple Panel derivative that lays out its children in a **circular** arrangement. It has some useful properties to allow some customization like the Orientation (Clockwise or Counterclockwise).

<img src="images/circularlayout.png" Width="250" />

### DockLayout

The DockLayout allows you to **dock** the child controls to the top, bottom, left or right. By default, the last control, if not given a specific dock position, will fill the remaining space. You can achieve the same with the Grid panel, but for the simpler situations, the DockLayout will be easier to use. Use the DockLayout whenever you need to dock one or several controls to one of the sides, like for dividing up the screen into specific areas.

<img src="images/docklayout.png" Width="250" />

### HexLayout

A panel that arranges the elements in a **honeycomb pattern**.

<img src="images/hexlayout.png" Width="250" />

### UniformGrid

The UniformGrid is just like the Grid, with the possibility of multiple rows and columns, but with one important difference: All rows and columns will have the **same size**. Use this when you need the Grid behavior without the need to specify different sizes for the rows and columns.

<img src="images/uniformgrid.png" Width="250" />

### WrapLayout

The WrapLayout will position each of its child controls next to the other, horizontally (default) or vertically, until there is no more room, where it will **wrap** to the next line and then continue. Use it when you want a vertical or horizontal collection controls that automatically wraps when there's no more room.

<img src="images/wraplayout.png" Width="250" />

## Feedback

Please use [GitHub issues](https://github.com/jsuarezruiz/xampane/issues) for questions or comments.

## Copyright and license

Code released under the [MIT license](https://opensource.org/licenses/MIT).