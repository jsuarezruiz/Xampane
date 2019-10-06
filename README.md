# Xampane

Xamarin.Forms **Layouts** library.

<img src="images/xampane.png" Width="150" />

### CircularLayout

The CircularLayout is a simple Panel derivative that lays out its children in a **circular** arrangement. It has some useful properties to allow some customization like the Orientation (Clockwise or Counterclockwise).

```
<xampane:CircularLayout
    Orientation="Clockwise">
    <BoxView Color="Black" CornerRadius="6" WidthRequest="6" HeightRequest="6" />       
    <BoxView Color="Red" CornerRadius="12" WidthRequest="12" HeightRequest="12" xampane:CircularLayout.Angle="0" xampane:CircularLayout.Radius="120" />
    <BoxView Color="Green" CornerRadius="12" WidthRequest="12" HeightRequest="12" xampane:CircularLayout.Angle="10" xampane:CircularLayout.Radius="120" />
    <BoxView Color="Blue" CornerRadius="12" WidthRequest="12" HeightRequest="12" xampane:CircularLayout.Angle="20" xampane:CircularLayout.Radius="120" />
    <BoxView Color="Yellow" CornerRadius="12" WidthRequest="12" HeightRequest="12" xampane:CircularLayout.Angle="30" xampane:CircularLayout.Radius="120" />
    <Label Text="1" xampane:CircularLayout.Angle="30" xampane:CircularLayout.Radius="90" />
    <Label Text="2" xampane:CircularLayout.Angle="60" xampane:CircularLayout.Radius="90" />
    <Label Text="3" xampane:CircularLayout.Angle="90" xampane:CircularLayout.Radius="90" />
    <Label Text="4" xampane:CircularLayout.Angle="120" xampane:CircularLayout.Radius="90" />
    <Label Text="5" xampane:CircularLayout.Angle="150" xampane:CircularLayout.Radius="90" />
    <Label Text="6" xampane:CircularLayout.Angle="180" xampane:CircularLayout.Radius="90" />
    <Label Text="7" xampane:CircularLayout.Angle="210" xampane:CircularLayout.Radius="90" />
    <Label Text="8" xampane:CircularLayout.Angle="240" xampane:CircularLayout.Radius="90" />
    <Label Text="9" xampane:CircularLayout.Angle="270" xampane:CircularLayout.Radius="90" />
    <Label Text="10" xampane:CircularLayout.Angle="300" xampane:CircularLayout.Radius="90" />
    <Label Text="11" xampane:CircularLayout.Angle="330" xampane:CircularLayout.Radius="90" />
    <Label Text="12" xampane:CircularLayout.Angle="360" xampane:CircularLayout.Radius="90" />
</xampane:CircularLayout>
```
<img src="images/circularlayout.png" Width="250" />

### DockLayout

The DockLayout allows you to **dock** the child controls to the top, bottom, left or right. By default, the last control, if not given a specific dock position, will fill the remaining space. You can achieve the same with the Grid panel, but for the simpler situations, the DockLayout will be easier to use. Use the DockLayout whenever you need to dock one or several controls to one of the sides, like for dividing up the screen into specific areas.

```
<xampane:DockLayout
    LastChildFill="False">
    <Button xampane:DockLayout.Dock="Top" Text="Top" HeightRequest="50"/>
    <Button xampane:DockLayout.Dock="Bottom" Text="Bottom" HeightRequest="50"/>
    <Button xampane:DockLayout.Dock="Left" Text="Left" WidthRequest="60"/>
    <Button xampane:DockLayout.Dock="Left" Text="Left" WidthRequest="60"/>
    <Button xampane:DockLayout.Dock="Right" Text="Right" WidthRequest="80"/>
    <Button xampane:DockLayout.Dock="Right" Text="Right" WidthRequest="80"/>
</xampane:DockLayout>
```
<img src="images/docklayout.png" Width="250" />

### HexLayout

A panel that arranges the elements in a **honeycomb pattern**.

```
<xampane:HexLayout
    RowCount="3"
    ColumnCount="3"
    Orientation="Vertical">
    <polygon:PolygonFrame xampane:HexLayout.Row="0" xampane:HexLayout.Column="1" OffsetAngle="90" BackgroundColor="Red"/>
    <polygon:PolygonFrame xampane:HexLayout.Row="0" xampane:HexLayout.Column="2" OffsetAngle="90" BackgroundColor="Green"/>
    <polygon:PolygonFrame xampane:HexLayout.Row="1" xampane:HexLayout.Column="0" OffsetAngle="90" BackgroundColor="Blue"/>
    <polygon:PolygonFrame xampane:HexLayout.Row="1" xampane:HexLayout.Column="1" OffsetAngle="90" BackgroundColor="Yellow"/>
    <polygon:PolygonFrame xampane:HexLayout.Row="1" xampane:HexLayout.Column="2" OffsetAngle="90" BackgroundColor="Orange"/>
    <polygon:PolygonFrame xampane:HexLayout.Row="2" xampane:HexLayout.Column="1" OffsetAngle="90" BackgroundColor="Purple"/>
    <polygon:PolygonFrame xampane:HexLayout.Row="2" xampane:HexLayout.Column="2" OffsetAngle="90" BackgroundColor="Pink"/>
</xampane:HexLayout>
```
<img src="images/hexlayout.png" Width="250" />

### UniformGrid

The UniformGrid is just like the Grid, with the possibility of multiple rows and columns, but with one important difference: All rows and columns will have the **same size**. Use this when you need the Grid behavior without the need to specify different sizes for the rows and columns.

```
<xampane:UniformGrid>
    <BoxView Color="Red" />
    <BoxView Color="Yellow" />
    <BoxView Color="Orange" />
    <BoxView Color="Purple" />
    <BoxView Color="Blue" />
    <BoxView Color="Green" />
    <BoxView Color="LightGreen" />
    <BoxView Color="Gray" />
    <BoxView Color="Pink" />
</xampane:UniformGrid>
```
<img src="images/uniformgrid.png" Width="250" />

### WrapLayout

The WrapLayout will position each of its child controls next to the other, horizontally (default) or vertically, until there is no more room, where it will **wrap** to the next line and then continue. Use it when you want a vertical or horizontal collection controls that automatically wraps when there's no more room.

```
<xampane:WrapLayout 
    Orientation="Vertical"
    Spacing="6"
    HorizontalOptions="Center">
    <BoxView Color="Red" />
    <BoxView Color="Yellow" />
    <BoxView Color="Orange" />
    <BoxView Color="Purple" />
    <BoxView Color="Blue" />
    <BoxView Color="Green" />
    <BoxView Color="LightGreen" />
    <BoxView Color="Gray" />
    <BoxView Color="Pink" />
</xampane:WrapLayout>
```
<img src="images/wraplayout.png" Width="250" />

## Feedback

Please use [GitHub issues](https://github.com/jsuarezruiz/xampane/issues) for questions or comments.

## Copyright and license

Code released under the [MIT license](https://opensource.org/licenses/MIT).