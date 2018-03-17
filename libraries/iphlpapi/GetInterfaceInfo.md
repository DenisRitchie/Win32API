<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : GetInterfaceInfo
Group: IP Helper - Library: iphlpapi    
***  


#### The GetInterfaceInfo function obtains a list of the network interface adapters on the local system.
***  


## Code examples:
[How to release and renew a lease on an IP address previously obtained through Dynamic Host Configuration Protocol (DHCP)](../../samples/sample_349.md)  

## Declaration:
```foxpro  
DWORD GetInterfaceInfo(
	PIP_INTERFACE_INFO pIfTable,
	PULONG dwOutBufLen
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER GetInterfaceInfo IN iphlpapi;
	STRING @ pIfTable,;
	LONG   @ dwOutBufLen  
```  
***  


## Parameters:
```txt  
pIfTable
[in] Pointer to a buffer that specifies a IP_INTERFACE_INFO structure that contains the list of adapters.

dwOutBufLen
[out] Pointer to a DWORD variable. If the buffer pointed to by the pIfTable parameter is NULL, or is not large enough to contain the list of adapters, GetInterfaceInfo receives the required size in this DWORD variable.  
```  
***  


## Return value:
If the function succeeds, the return value is NO_ERROR.  
***  


## Comments:
Normally this functionality is achieved through <Strong>IPCONFIG /all</Strong> call.  
  
***  
