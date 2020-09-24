<div align="center">

## BMTEncode


</div>

### Description

Encode/Decode a string. (BMTEncode refined version). If f.ex. enter AA the 2

output chars wont be the same.
 
### More Info
 
Textstring = text to Encode/Decode

value = 0 or 1 for either Encode/Decode

String


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Y'll never know](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/y-ll-never-know.md)
**Level**          |Unknown
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[String Manipulation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/string-manipulation__1-5.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/y-ll-never-know-bmtencode__1-1363/archive/master.zip)





### Source Code

```
'* Sorry for stealing code, but I couldn't help it when I saw the garbage
'* routine called BMTEncrypt.
Function BTMEncrypt(text, types)
 For god = 1 To Len(text)
   If types = 0 Then
     Current$ = Asc(Mid(text, god, 1)) - god
   Else
     Current$ = Asc(Mid(text, god, 1)) + god
   End If
   Process$ = Process$ & Chr(Current$)
 Next god
 BTMEncrypt = Process$
End Function
```

