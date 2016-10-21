# Address

Mandrill now supports dynamic layout creation, thanks to a piece of Java Script library called Gridster. What Gridster is doing for us, is that it divides the whole page into a grid of cells. Each cell is <b>100px x 100px</b>. Starting in the top/left corner of the screen, each chart, image, legend added to the report and visualized in the window, now has an address. Rows and columns are numbered sequentially so top/left is [1,1]. Kind of like this: 

![](MiscNodes/Address/address-01.png)

Something to keep in mind when specifying the address for a chart. It's address is relative to charts top/left corner. So for example telling a chart to be slotted at [2,3] would result in something like this: 

![](MiscNodes/Address/address-02-01.png)
