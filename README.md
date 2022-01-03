# utils_for_keyboradrate_for_sc2

autohotkey写的暴兵宏.
 F6 光速买地雷运输机和50枪兵. 然后自动再选择1部队
 
 F5光速买50枪兵
 
 
 
 
 首先需要用keyrate.exe让输入加速. 
 设置方法cmd里面输入

	下载keyrate软件设置键盘速度.
	keyrate.exe 160 10
	就是上面这个参数,设置其他更快也没效果.会耽误输入.不要自己改参数.
 
 参考  	https://github.com/EricTetz/keyrate/releases
 
 
 
 
 ```


/*
#IFWinActive 星际争霸


F5::


Send, {backspace}

MouseClickDrag, left,  A_ScreenWidth/2-300, A_ScreenHeight/2 -300, A_ScreenWidth/2+300,  A_ScreenHeight/2 +300 ,1

Send, {v}

MouseClick, left,  A_ScreenWidth/2  , A_ScreenHeight/2 -10,1,1  ;居中点一下

return 

*/










;F6 4个地雷2个运输机,50个枪兵一键建造
#IFWinActive 星际争霸       


F6::
SendInput, {3}
SendInput, {tab 2}
SendInput, dd
SendInput, {tab 2}
SendInput, dddd
SendInput, {tab 2}
SendInput, 3adadadaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa



Send, {1}



return 






;写人族暴兵,配合keyrate软件,光速输入.
#IFWinActive 星际争霸       


F5::

SendInput, {3}
SendInput, {tab 2}

SendInput, {tab 2}

SendInput, {tab 2}
SendInput, 3adadadaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa



Send, {1}



return 





;之前设置的是空格是选中一个农民,ctrk+空格是全部农民.直接改建空格是选中全部空闲农民更方便.;需要把设置里面快捷键
;中的选中空闲农民设置为空格.
#IFWinActive 星际争霸       


$Space::



Send, ^{space}



return 

```


最后附上我的星际心得:










2021-12-02,14点16
学星际运营:
	学下面这个视频就够了!!!!!!!
	https://www.bilibili.com/video/BV1BQ4y1i7N2
	学习运营的方法.一定要看自己rep哪里错了,就记下来.每次改进一点.一定一定要看自己rep
	重要点一个是气矿下的时机, 一个是补房子别卡人口.


星际shift编队技巧:
	Shift键能向已有编队里面添加单位，
	具体操作时选中想要添加的单位，如果想要添加到1队里，就按Shift + 1

	连弩是. 右键点一个毒爆然后shift a鼠标左键把毒爆都点一遍.因为shift右键一旦没点中,
	点地板了那就废了.


	把编队,单位管理,上一个子编组修改成caplock
	这样控制部队埋雷按caplock和e即可.

	编屏设置为shift+f1-4
	4基地加be加va，5兵营重工机场
	
	把s 和h 互换。
	建筑 升起和降落 全部换成w 两个全换成w
	空闲农民空格
	警告信息alt
	原来的f2 我建议放在` 键
	
	
	1 2 编部队

	3 编所有造兵建筑 tab键切换

	4编所有主基地+攻防 造农民 撒雷达 匡罗等等

	把攻防编一起的好处是你每次切到主基地的时候都可以看到攻防升好了没有 避免遗忘

	5键编多线骚扰的解放者 或者小部队






游戏设置

	画质都调到最低,这样延迟最低,也没有阴影看的更确切.有阴影容易看不起.
	显示模式一定全屏,gamma调高.改成受伤显示血条.这样不容易遮挡画面.
	语音只开音效.去掉背景音乐.
	兴奋剂持续时间经过测试是11秒.攻速移动速度都加百分之50




	星际如何离线打电脑.
	首先去自定义-----对战里面下载好地图.就是玩一次.
	然后拔网线.转圈一会儿,点击离线模式运行.
	之后再进入自定义就可以打电脑了.
	rpg地图同理一样.在游戏大厅下好地图即可.
	
	
	https://github.com/EricTetz/keyrate/releases
	下载keyrate软件设置键盘速度.
	keyrate.exe 160 10
	就是上面这个参数,设置其他更快也没效果.会耽误输入.不要自己改参数.




然后一直循环的操作是
运营, 买农民, 暴兵 再运营再农民暴兵.....循环下去
运营指的是走下面的流程.

目前最优方案
火车女妖套路:
	2农民
	bs
	2农民
	bb br
	3农民 星轨,死神, bc,
	bs, 矿罗,农民,枪兵 (这里面bs防止卡枪兵人口,和封路口)
	vf 双倍 bc 
	vs br 科技 隐形 科技 
	8火车2女妖
	2bb  兴奋剂 2br 2be  2bb
	3矿满了, vf 3bb 开4矿


tvp:3兵营
	bb br 星轨 枪 bc (一个细节是18农民去对面二矿看一下,如果没有二基地.我们就不下二基地.)
	双 bs  
	2bb 兴盾 br be
	vf br
	vs 双 bc
	2bb

tvz: 2兵营(这个是最核心的战术)


	bs bb br 设置农民shift2矿 bb集结点到对面 星轨死神bc  这一行是标准前期最优开
	bb 矿罗 买农民  bs  双 br (这4个要背下来最后这个br我总忘)
	vf bb挂科 兴 
	
	vs  vf挂双倍  调节农民集结点 vf挂科技 盾牌
	3bs  bc 
	2船兵出发.
	2br 2be 2bb


tvt: 死火流
	bs bb 2br
	星轨死神bs
	vf 4采气 双 bc bs
	vs 调节农民集结点 vf挂科技 br

https://www.webacg.com/game/gl/297341.html
运营理解:
	1.一般都是第二个出兵建筑和第三个出兵建筑之间放下第二个气矿. 第二个建筑之前放bs,因为第二个出兵建筑出完就开始要大量气了.
	2.2矿3兵营,3矿兵营. 一般产兵建筑弄好了就补3,4气.和2be,一攻一防升级到一半下va
	3.tvt后期大和
	  tvz后期靠地雷,鬼兵
	  tvp后期靠解放,鬼兵




















 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
