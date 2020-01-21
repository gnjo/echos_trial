
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
2>{$$$}
//
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
