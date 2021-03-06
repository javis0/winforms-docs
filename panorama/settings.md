---
title: Settings
page_title: Settings | UI for WinForms Documentation
description: Settings
slug: winforms/panorama/settings
tags: settings
published: True
position: 5
previous_url: panorama-settings
---

# Settings

## 

The RadPanorama control uses a __GridLayout__ element to display its tiles. By setting the __CellSize__ property, you can change the default size of a single cell which is also the default size of a tile. You can set this property either in the Smart Tag or in Properties window.

Tile can be reordered via Drag and Drop. To allow or disallow this, set the __AllowDragDrop__ property in the Properties window or via code:

#### Allow drag and drop

{{source=..\SamplesCS\Panorama\PanoramaGettingStarted.cs region=AllowDragDrop}} 
{{source=..\SamplesVB\Panorama\PanoramaGettingStarted.vb region=AllowDragDrop}} 

````C#
this.radPanorama1.AllowDragDrop = true;

````
````VB.NET
Me.RadPanorama1.AllowDragDrop = True

````

{{endregion}}

RadPanorama uses a fixed number of rows, but the control changes the number of columns at runtime to allow more flexible drag and drop operations. To set the number of rows, set the __RowsCount__ property either through the Properties window or through the Smart Tag menu. You can also specify a minimum number of columns by setting the __MinimumColumns__ property.

#### Set RowCount and minimum number of columns

{{source=..\SamplesCS\Panorama\PanoramaGettingStarted.cs region=RowAndCol}} 
{{source=..\SamplesVB\Panorama\PanoramaGettingStarted.vb region=RowAndCol}} 

````C#
this.radPanorama1.RowsCount = 5;
this.radPanorama1.MinimumColumns = 5;

````
````VB.NET
Me.RadPanorama1.RowsCount = 5
Me.RadPanorama1.MinimumColumns = 5

````

{{endregion}}