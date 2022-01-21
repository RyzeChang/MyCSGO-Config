# CSGO Settings



## Launch Options


```
-worldwide -high -freq 60 +fps_max 0 -novid -nojoy +exec config.cfg -console -language english -nohltv 
```
-   **-autoconfig** - This command lets you restore config file settings to deafult.
  
-   **+exec file name** - Launch option that launching the config with game settings (.cfg). The file should be placed in folder "Steam\SteamApps\common\Counter-Strike Global Offensive\csgo\cfg".



## Config 

```
hud_scaling 0.95 // 整体hud比例，调到最大

cl_hud_radar_scale 1.3 //雷达大小，调到最大

cl_radar_scale 0.4 // (雷达显示地图范围，数字越小显示地图范围越大，但是小一点的地图最好调到0.7以上，比如seaside\nuke)

cl_radar_always_centered 0 //(这个个人喜好，不显示居中不会留太多黑边)

cl_radar_icon_scale_min 0.4 //(设置显示队友那些点点的大小，一般0.4以下就好，0.6的话点点太大，容易重叠)
```





## autoexec.cfg

```
// 客户端常用设置
// 穿墙看队友，1是看名字，2是看装备+名字，0是关闭
cl_teamid_overhead_mode "2"  
// 关闭固定死亡视角
cl_disablefreezecam 
// Reduce gun shifting when crouching
cl_viewmodel_shift_left_amt "0"
cl_viewmodel_shift_right_amt "0"
// Reduce gun and scope shifting/bobbing when moving
cl_bobcycle "0"
cl_bob_lower_amt "0"
cl_bobamt_lat "0"
cl_bobamt_vert "0"

// 准星设置
cl_crosshair_drawoutline 0 
cl_crosshairalpha "250"
cl_crosshaircolor "4"
cl_crosshaircolor_b "165" 
cl_crosshaircolor_g "255" 
cl_crosshaircolor_r "0" 
cl_crosshairdot "1"
cl_crosshairscale "120"
cl_crosshairsize "1"
cl_crosshairthickness "0"
cl_crosshairusealpha "1"
cl_crosshairgap -3
cl_crosshairstyle 4

// Radar雷达
cl_radar_always_centered "1" 雷达是否居中（1是，0不是）
cl_radar_rotate "1" 雷达是否旋转 0关 1开
cl_radar_scale "0.5" 雷达缩放（0.25-1越小，小地图看到的东西越小越多）
cl_radar_icon_scale_min "0.75" 雷达人物标点大小
cl_radar_square_with_scoreboard "0 "开启计分板雷达是否变成方形 0关 1开 

// Jumpthrow T键可以改成任何你想使用的键，意为绑定T键为“跳投”，只要切出指定道具后，按住鼠标左键，保持投掷物呈拉开保险的状态，之后按下T即可实现投掷物的标准跳投。
alias "+jumpthrow" "+jump;-attack";
alias "-jumpthrow" "-jump";
bind "T" "+jumpthrow"

// Jump+crouch 一建跳蹲
alias +cjump "+jump; +duck"
alias -cjump "-jump; -duck"
bind "space" "+cjump”

// ClearF键清除血迹指令
bind "f" "+lookatweapon; r_cleardecals"

ECHO ================================================
ECHO ===[        Autoexec CFG loaded!          ]=====
ECHO ===[        Good luck have fun!           ]=====
ECHO ================================================
```
An autoexec is simply a text file with a list of commands that are executed when you start CS:GO. This is useful because often commands will return to their default value when you restart your game, commands in your autoexec will keep their values.

After placing your autoexec file (named autoexec.cfg) in the "Steam\SteamApps\common\Counter-Strike Global Offensive\csgo\cfg" folder, set the following launch option to make it work:

+exec autoexec.cfg [COPY](https://totalcsgo.com/launch-options#)

If your autoexec file isn't named autoexec.cfg, replace autoexec.cfg with the name of your autoexec file.


Niko autoexec.cfg

```
voice_mixer_volume 1


snd_mixahead "0.05"
snd_headphone_pan_exponent "2"
snd_musicvolume "0.0"
snd_tensecondwarning_volume "0.04"


cl_cmdrate "128"
cl_updaterate "128"
rate "786432"
cl_interp "1"
cl_interp_ratio "2"


m_rawinput "1"
m_mouseaccel1 "0"
m_mouseaccel2 "0"


r_drawtracers_firstperson "0"
cl_autowepswitch "0"
hud_showtargetid "1"
hud_scaling "0.95"
net_graph "0"
fps_max "700"
cl_autohelp "0"
cl_showhelp "0"


bind kp_end "BUY vest"
bind kp_downarrow "BUY vesthelm"
bind kp_pgdn "BUY flashbang"
bind kp_leftarrow "BUY hegrenade"
bind kp_5 "BUY smokegrenade"
bind kp_rightarrow "BUY defuser"
bind kp_home "BUY molotov; BUY incgrenade"
bind kp_uparrow "BUY decoy"
bind c "USE weapon_molotov; USE weapon_incgrenade"
bind kp_ins "Buy ak47;buy m4a1"
bind kp_enter "Buy p250"


net_graph 1
net_graphpos 2


alias "+jumpthrow" "+jump;-attack"
alias "-jumpthrow" "-jump"
bind "mouse4" "+jumpthrow" 
bind "mouse5" "toggle cl_radar_scale 0.35 1"


alias +jumpthrow "+jump; -attack; -attack2"
alias -jumpthrow "-jump"
bind h "+jumpthrow"


bind v r_cleardecals 


alias "warmup"  "rcon ammo_grenade_limit_total 0;rcon bot_kick;rcon mp_buytime 9999999;rcon mp_freezetime 0;rcon mp_maxmoney 50000000;rcon mp_startmoney 50000000;r


```




https://dmarket.com/zh/ingame-items/item-list/csgo-skins

https://www.bilibili.com/video/BV13Z4y1w7AT

https://www.bilibili.com/video/BV1MU4y1b7LP

https://www.bilibili.com/video/BV19h411Q7DZ

## 参考

1. [Esports database for pro settings](https://prosettings.net/)
2. https://www.wevg.org/archives/csgo-config-guide/
3. https://github.com/marcus5746/CSGO-USEFUL-CFGs-/blob/main/autoexec.cfg
4. https://prosettings.net/counterstrike/niko/
5. https://prosettings.net/library/best-cs-go-binds/
6. https://www.zhihu.com/column/c_1321089685633028096
7. [CSGO practice config - cfg, bots, show trajectory, bullet impacts (leetify.com)](https://blog.leetify.com/csgo-practice-config/)
8. [The Best CSGO Binds (leetify.com)](https://blog.leetify.com/best-csgo-binds/)
9. https://www.one-tab.com/page/pLgWqPpRSoOaJmWenYAP7w
10. https://prosettings.net/cs-go-best-settings-options-guide/
11. https://prosettings.net/library/how-to-use-cs-go-config-autoexec/

