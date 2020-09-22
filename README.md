<div align="center">

## Simple & Secure encryption


</div>

### Description

SO SIMPLE, SOOOOO STRONG... Just try to find a pattern in this encryption.... Try sending it a string containing all the same letters, are you amazed by the outcome??? (! KEEP IN MIND THAT ANYONE WITH A CONNECTION TO THE INTERNET HAS ACCESS TO THIS CODE. SO THE ENCRYPTION CAN BE CRACKED. IF WHAT YOU ARE ENCRYPTING IS VERY IMPORTANT, MAKE A MINOR CHANGE TO THE CODE TO AVOID PEOPLE CRACKING YOUR IMPORTANT INFO !)
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Dave Katrowski](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/dave-katrowski.md)
**Level**          |Intermediate
**User Rating**    |4.0 (8 globes from 2 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0, VB Script, ASP \(Active Server Pages\) 
**Category**       |[Encryption](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/encryption__1-48.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/dave-katrowski-simple-secure-encryption__1-9310/archive/master.zip)

### API Declarations

```
'none
```


### Source Code

```
Dim s As String, i As Integer
If Left(Text1, 3) = "DMK" Then
Text1 = Right(Text1, Len(Text1) - 3)
For i = 1 To Len(Text1)
If i <= 100 Then
s = s & Chr(Asc(Mid(Text1, i, 1)) - 128 Mod i)
Else
s = s & Chr(Asc(Mid(Text1, i, 1)) - 128 Mod i / 10)
End If
Next
Else
For i = 1 To Len(Text1)
If i <= 100 Then
s = s & Chr(Asc(Mid(Text1, i, 1)) + 128 Mod i)
Else
s = s & Chr(Asc(Mid(Text1, i, 1)) + 128 Mod i / 10)
End If
Next
s = "DMK" & s
End If
Text1 = s
```

