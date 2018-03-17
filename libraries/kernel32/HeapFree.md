<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : HeapFree
Group: Memory Management - Library: kernel32    
***  


#### The HeapFree function frees a memory block allocated from a heap by the HeapAlloc or HeapReAlloc function.
***  


## Code examples:
[Using the heap of the calling process to allocate memory blocks](../../samples/sample_199.md)  

## Declaration:
```foxpro  
BOOL HeapFree(
  HANDLE hHeap,  // handle to heap
  DWORD dwFlags, // heap free options
  LPVOID lpMem   // pointer to memory
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER HeapFree IN kernel32;
	INTEGER hHeap,;
	INTEGER dwFlags,;
	INTEGER lpMem  
```  
***  


## Parameters:
```txt  
hHeap
[in] Specifies the heap whose memory block the function frees. This parameter is a handle returned by the HeapCreate or GetProcessHeap function.

dwFlags
[in] Specifies several controllable aspects of freeing a memory block.

lpMem
[in] Pointer to the memory block to free. This pointer is returned by the HeapAlloc or HeapReAlloc function.
  
```  
***  


## Return value:
If the function succeeds, the return value is nonzero. If the function fails, the return value is zero.  
***  
