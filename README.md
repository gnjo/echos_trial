# echos
memory input macro

```
echos.add(macro).add(macro2).add(macro3)
 .key('w,a,s,d,j,k,i,l,u,o') //^,<,v,>,a,b,x,y,l,r
 .run((mode,log,info,seln,ec)=>{},20) //always start '#echos'
 
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
{1}>>>#aiuewo //jump
{1}>>>{$$jumpback} //jumpback

$$$ return
$$0...9 return0
$$jumpback //11 number jumpbackline
```
```
#echos
>hello echos
>{ec.mode}
>{ec.line}
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
{$00=$$jumpback} //stock the oldjump
{1}>>>{$00}

```
