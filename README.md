# echos
memory input macro

```
let drawer=(mode,log,info,seln,ec)=>{}
echos.add(macro).add(macro2).add(macro3)
 .key('w,a,s,d,j,k,i,l,u,o') //^,<,v,>,a,b,x,y,l,r
 .run(drawer,20) //always start '#echos'
 
 //mode =sel|mes|free
 //waitcount
 //if message buffering waitcount +=4
```
```
>press anykey message
>>not press message
i>output info
?>select call  //use info area
{/*javascript world*/}
{{{}}} //$$$ input
{1}>>>#aiuewo //jump
{1}>>>{ec.jumpback} //jumpback
{1}>>>### //same

$$$ return
$$0...9 return0
### //number jumpbackline
```
```
#echos
>hello echos
>{ec.mode}
>{ec.line}
>{ec.logMaxWidth}
>{ec.logMaxLines}
* //waitcount +=4, if ** is +8
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

```
let n=5
let a='aiueoaiueoaiueo'.match(new RegExp('.{'+n+'}','g')) //  /.{5}/g
```

```
//double jumps
{$00=ec.jumpback} //stock the old jump line
{1}>>>{$00}

```
