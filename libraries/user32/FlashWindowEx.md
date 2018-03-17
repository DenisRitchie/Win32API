<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : FlashWindowEx
Group: Error Handling - Library: user32    
***  


#### The FlashWindowEx function flashes the specified window. It does not change the active state of the window.
***  


## Code examples:
[Using FlashWindowEx to flash the taskbar button of the VFP application](../../samples/sample_271.md)  

## Declaration:
```foxpro  
BOOL FlashWindowEx(
  PFLASHWINFO pfwi  // flash status information
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER FlashWindowEx IN user32;
	STRING pfwi
  
```  
***  


## Parameters:
```txt  
pfwi
[in] Pointer to the FLASHWINFO structure.  
```  
***  


## Return value:
The return value specifies the window"s state before the call to the FlashWindowEx function.  
***  


## Comments:
Windows NT/2000/XP: Included in Windows 2000 and later.  
Windows 95/98/Me: Included in Windows 98 and later.  
  
***  
