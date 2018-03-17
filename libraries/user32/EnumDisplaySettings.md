<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : EnumDisplaySettings
Group: Device Context - Library: user32    
***  


#### The EnumDisplaySettings function retrieves information about one of the graphics modes for a display device. To retrieve information for all the graphics modes of a display device, make a series of calls to this function.
***  


## Code examples:
[How to change display settings: screen resolution, screen refresh rate](../../samples/sample_374.md)  
[How to detect if additional monitor is connected and active](../../samples/sample_542.md)  

## Declaration:
```foxpro  
BOOL EnumDisplaySettings(
  LPCTSTR lpszDeviceName,  // display device
  DWORD iModeNum,          // graphics mode
  LPDEVMODE lpDevMode      // graphics mode settings
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER EnumDisplaySettings IN user32;
	STRING    lpszDeviceName,;
	INTEGER   iModeNum,;
	STRING  @ lpDevMode  
```  
***  


## Parameters:
```txt  
lpszDeviceName
[in] Pointer to a null-terminated string that specifies the display device about whose graphics mode the function will obtain information.

iModeNum
[in] Specifies the type of information to retrieve.

lpDevMode
[out] Pointer to a DEVMODE structure into which the function stores information about the specified graphics mode.  
```  
***  


## Return value:
If the function succeeds, the return value is nonzero.  
***  


## Comments:
MSDN: The function fails if iModeNum is greater than the index of the display device"s last graphics mode. As noted in the description of the iModeNum parameter, you can use this behavior to enumerate all of a display device"s graphics modes.   
  
***  
