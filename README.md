# echos
memory input macro

```
let drawer=(mode,log,info,seln,ec)=>{}
echos.add(macro).add(macro2).add(macro3)
 .key('w,a,s,d,j,k,i,l,u,o') //^,<,v,>,a,b,x,y,l,r
 .run(drawer,20) //always start '#echos'
 
 //mode =sel|mes|free
 //waitcount
 //if message buffering waitcount +1
```
```
>press anykey message mode='mes'
>>not press message mode='mes'
i>output info mode='free'
k> keywait keep the mode
?>select call  //use info area mode='sel'
* //wait keep the mode 
{/*javascript world*/} mode='free'
{{{}}} //$$$ input mode='free'
{1}>>>#aiuewo //jump mode='free'
{1}>>>{ec.jumpback} //jumpback  mode='free'
{1}>>>### //same  mode='free'

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


```
#walk
//keywait order
k>
i>{$$k}
{1}>>>#walk
```



