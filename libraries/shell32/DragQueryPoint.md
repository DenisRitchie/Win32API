<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : DragQueryPoint
Group: Shell Functions - Library: shell32    
***  


#### Retrieves the position of the mouse pointer at the time a file was dropped during a drag-and-drop operation.
***  


## Code examples:
[Dragging files from Explorer window and dropping them on FoxPro control (requires VFP9)](../../samples/sample_323.md)  

## Declaration:
```foxpro  
BOOL DragQueryPoint(
	HDROP hDrop,
	LPPOINT lppt
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER DragQueryPoint IN shell32;
	INTEGER  hDrop,;
	STRING @ lppt
  
```  
***  


## Parameters:
```txt  
hDrop
Identifier of the structure that describes the dropped file.

lppt
Address of a POINT structure that the function fills with the coordinates of the mouse pointer at the time the file was dropped.  
```  
***  


## Return value:
Returns nonzero if the drop occurred in the client area of the window, or zero if the drop did not occur in the client area of the window.   
***  


## Comments:
The window for which coordinates are returned is the window that received the WM_DROPFILES message.   
  
See also: DragAcceptFiles, DragQueryFile.  
  
***  
