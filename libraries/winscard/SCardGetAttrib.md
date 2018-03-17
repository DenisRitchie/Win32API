<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : SCardGetAttrib
Group: Authentication - Library: winscard    
***  


#### Gets the current reader attributes for the given handle. It does not affect the state of the reader, driver, or card.

***  


## Declaration:
```foxpro  
LONG SCardGetAttrib(
  __in     SCARDHANDLE hCard,
  __in     DWORD dwAttrId,
  __out    LPBYTE pbAttr,
  __inout  LPDWORD pcbAttrLen
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE LONG SCardGetAttrib IN Winscard;
	INTEGER hCard,;
	LONG dwAttrId,;
	STRING @pbAttr,;
	LONG @pcbAttrLen  
```  
***  


## Parameters:
```txt  
hCard [in]
Reference value returned from SCardConnect.

dwAttrId [in]
Identifier for the attribute to get.

pbAttr [out]
Pointer to a buffer that receives the attribute whose ID is supplied in dwAttrId.

pcbAttrLen [in, out]
Length of the pbAttr buffer in bytes, and receives the actual length of the received attribute.  
```  
***  


## Return value:
Returns SCARD_S_SUCCESS (0) or error code.  
***  


## Comments:
In Winsmcrd.h file the SCARD_ATTR_VALUE macro is used to define the attribute constants.  
  
<div class="precode">#define SCARD_ATTR_VENDOR_NAME  
	SCARD_ATTR_VALUE(SCARD_CLASS_VENDOR_INFO, 0x0100)  
</div>  
The statement above can be translated into VFP code as follows:  
  
<div class="precode">#DEFINE SCARD_ATTR_VENDOR_NAME;  
	BITOR(BITLSHIFT(SCARD_CLASS_VENDOR_INFO, 16), 0x0100)</div>  
  
***  
