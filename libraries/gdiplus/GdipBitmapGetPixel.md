<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : GdipBitmapGetPixel
Group: GDI+ Bitmap - Library: gdiplus    
***  


#### Gets the color value of an individual pixel.
***  


## Code examples:
[GDI+: Color Transparency](../../samples/sample_549.md)  

## Declaration:
```foxpro  
GpStatus WINGDIPAPI GdipBitmapGetPixel(
	GpBitmap* bitmap,
	INT x, INT y, ARGB *color)  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER GdipBitmapGetPixel IN gdiplus;
	INTEGER gdibitmap,;
	INTEGER x,;
	INTEGER y,;
	LONG @argbcolor  
```  
***  


## Parameters:
```txt  
gdibitmap
[in] Handle to a GDI bitmap.

x
[in] Integer X-coordinate of pixel to get.

y
[in] Integer Y-coordinate of pixel to get.

argbcolor
[out] ARGB color value of the pixel.  
```  
***  


## Return value:
Returns 0 on success.  
***  


## Comments:
See also: GdipBitmapSetPixel   
  
***  
