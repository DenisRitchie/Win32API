<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : GetCurrentDirectory
Group: File Management - Library: kernel32    
***  


#### The GetCurrentDirectory function retrieves the current directory for the current process.

***  


## Code examples:
[Current directory of the application](../../samples/sample_004.md)  

## Declaration:
```foxpro  
DWORD GetCurrentDirectory(
  DWORD nBufferLength,  // size of directory buffer
  LPTSTR lpBuffer       // directory buffer
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER GetCurrentDirectory IN kernel32;
	INTEGER   nBufferLength,;
	STRING  @ lpBuffer
  
```  
***  


## Parameters:
```txt  
nBufferLength
[in] Specifies the length, in TCHARs, of the buffer for the current directory string. The buffer length must include room for a terminating null character.

lpBuffer
[out] Pointer to the buffer that receives the current directory string. This null-terminated string specifies the absolute path to the current directory.  
```  
***  


## Return value:
If the function succeeds, the return value specifies the number of characters written to the buffer, not including the terminating null character  
***  


## Comments:
The difference between this function and SYS(2003) is next to negligible if any.  
  
See also: SetCurrentDirectory, GetFullPathName   
  
***  
