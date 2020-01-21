# echos
memory input macro

```
echos.add(macro).add(macro2).add(macro3)
 .key('w,a,s,d,j,k,i,l,u,o') //^,<,v,>,a,b,x,y,l,r
 .run((mode,mes,sel,seln,ec)=>{},20) //always start '#echos'
 
 //mode =sel|mes|free
 
```

```
#echos
>hello echos
>{ec.mode}
>{ec.line}
* //wait 50ms, if ** is 100ms
#jump1
{{{
a
i
u
e
other
}}}
?>{$$$}
{1}>>>#jump1
```
