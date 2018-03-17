<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : FindWindowEx
Group: Window - Library: user32    
***  


#### Retrieves a handle to a window whose class name and window name match the specified strings. The function searches child windows, beginning with the one following the specified child window.
***  


## Code examples:
[Scanning a hierarchy of child windows down from the Windows Desktop](../../samples/sample_045.md)  
[How to control Adobe Reader 9.0 (SDI mode) from VFP application](../../samples/sample_550.md)  

## Declaration:
```foxpro  
HWND FindWindowEx(
	HWND hwndParent,
	HWND hwndChildAfter,
	LPCTSTR lpszClass,
	LPCTSTR lpszWindow
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER FindWindowEx IN user32;
	INTEGER  hwndParent,;
	INTEGER  hwndChildAfter,;
	STRING @ lpszClass,;
	STRING @ lpszWindow
  
```  
***  


## Parameters:
```txt  
hwndParent
[in] Handle to the parent window whose child windows are to be searched.

hwndChildAfter
[in] Handle to a child window. The search begins with the next child window in the Z order.

lpszClass
[in]
Pointer to a null-terminated string that specifies the class name or a class atom created by a previous call to the RegisterClass or RegisterClassEx function.

lpszWindow
[in] Pointer to a null-terminated string that specifies the window name (the window"s title). If this parameter is NULL, all window names match.  
```  
***  


## Return value:
If the function succeeds, the return value is a handle to the window that has the specified class and window names.  
***  
