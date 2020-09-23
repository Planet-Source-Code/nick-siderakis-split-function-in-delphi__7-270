<div align="center">

## Split Function in Delphi


</div>

### Description

Hey this function just emulates the Visual Basic function that we know and love &#8220;<b>split</b>&#8221;!!! You use it the same way you would have in vb.<br><i>

avar := split('string to break up',' ',2);</i><br>

That will return avar as &#8220;to&#8221; that&#8217;s it, have fun and please vote!!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Nick Siderakis](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/nick-siderakis.md)
**Level**          |Intermediate
**User Rating**    |4.5 (36 globes from 8 users)
**Compatibility**  |Delphi 5, Delphi 4, Pre Delphi 4
**Category**       |[String Manipulation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/string-manipulation__7-5.md)
**World**          |[Delphi](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/delphi.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/nick-siderakis-split-function-in-delphi__7-270/archive/master.zip)





### Source Code

```
<pre><fontsize=2>function split(input:string;schar:char;s:integer):string;
var
   i,n:integer;
   schop: string;
begin
   n := 1;
   for i := 1 to length(input) do
   begin
     if (input[i] = schar) then
     begin
       inc(n);
       if n = s then
       split := schop
       else
       schop := '';
       end
     else
       schop := schop + input[i];
     end;
end;</pre>
```

