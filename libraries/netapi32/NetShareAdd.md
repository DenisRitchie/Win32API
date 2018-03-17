<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : NetShareAdd
Group: Network Management - Library: netapi32    
***  


#### Shares a server resource.
***  


## Code examples:
[How to enumerate, add and delete shares on the local computer (WinNT/XP)](../../samples/sample_351.md)  

## Declaration:
```foxpro  
NET_API_STATUS NetShareAdd(
	LPWSTR servername,
	DWORD level,
	LPBYTE buf,
	LPDWORD parm_err
);
  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER NetShareAdd IN netapi32;
	STRING servername,;
	LONG lvl,;
	STRING @buffer,;
	LONG @parm_err
  
```  
***  


## Parameters:
```txt  
servername
[in] Pointer to a string that specifies the DNS or NetBIOS name of the remote server on which the function is to execute.

level
[in] Specifies the information level of the data (2, 502).

buf
[in] Pointer to the buffer that specifies the data.

parm_err
[out] Pointer to a value that receives the index of the first member of the share information structure that causes the ERROR_INVALID_PARAMETER error.  
```  
***  


## Return value:
If the function succeeds, the return value is NERR_Success (0).  
***  


## Comments:
If the <Em>servername</Em> parameter is NULL, the local computer is used.  
  
***  
