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
$$k latest key
$$n latest select number
$$nn  selecting message number $o[$$nn] // -1 is disable
$$o output message 
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

```
#echos
//entrypoint


{1}>>>#map

#map
//add the map
//扉は、色で示される。黒茶赤橙黄緑青紫灰白
//一方通行扉は、東西南北。侵入できる方向を示す。
//自動移動床は、上下左右。
//イベントは、人物謎。
//床効果、毒、暗。イベントマスを床効果にする事は出来ない。
//特に必要ない場合、扉は＋、イベントは！、床は・で示す。
{{{
壁壁＋壁壁壁
・・！・・・
壁壁＋壁壁壁
}}}
{$$b[0]=$$$}
*
{1}>>>#city

#city
{$$n=0}
i0>cityimage
i1>citycenter
{{{
inn
temple
labyrinth
}}}
?2>{$$$}
//output 2 is selecting
//$$o[2]
{$$k==='b'}>>>#city
{$$n===0}>>>#inn
{$$n===1}>>>#temple
{$$n===2}>>>#B01X00Y00
*
{1}>>>#city

#walk
k>
1>{$$k}
{$$p=fn.walk($$p,$$k)}
//$$p={x,y,z,v,a0,a1}//a0 is ex)#B01X00Y00.W , a1 is ex)#B01X00Y00
{fn.isJump($$p.a0)}>>>{$$p.a0}
{fn.isJump($$p.a1)}>>>{$$p.a1}
{1}>>>#walk

#B00X00Y00
i0>aaaaa  //background image
i1>bbbbb  //center image
>{$$p.a0}
k>
*
{1}>>>#walk

```

