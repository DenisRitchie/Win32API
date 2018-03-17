<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : GetAsyncKeyState
Group: Keyboard Input - Library: user32    
***  


#### The GetAsyncKeyState function determines whether a key is up or down at the time the function is called, and whether the key was pressed after a previous call to GetAsyncKeyState. 
***  


## Code examples:
[Reading the state of mouse buttons within DO WHILE loop](../../samples/sample_280.md)  
[GDI+: Implementing image scrolling with inertia](../../samples/sample_595.md)  

## Declaration:
```foxpro  
SHORT GetAsyncKeyState(
  int vKey   // virtual-key code
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER GetAsyncKeyState IN user32;
	INTEGER vKey  
```  
***  


## Parameters:
```txt  
vKey
[in] Specifies one of 256 possible virtual-key codes.

  
```  
***  


## Return value:
If the function succeeds, the return value specifies whether the key was pressed since the last call to GetAsyncKeyState, and whether the key is currently up or down.  
***  


## Comments:
Check list of <a href="http://msdn.microsoft.com/en-us/library/ms645540(v=vs.85).aspx">Virtual-Key Codes</a> on the MSDN.   
  
***  
