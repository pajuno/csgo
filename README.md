//######################################
//
// ZeroNinja's CS:GO config para modo competitivo - geralmente este arquivo deve estar em C:\Program Files (x86)\Steam\SteamApps\common\Counter-Strike Global Offensive\csgo\cfg
// Baseado no autoexec.cfg http://www.spddl.de/csgo/hud/competitivehud
//
// ¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
// INSTALL/INSTALACAO:
// ¯¯¯¯¯¯¯
// Put the File "autoexec.cfg" into the following folder:
//
// ...\Steam\steamapps\common\Counter-Strike Global Offensive\csgo\cfg
//
// ¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯
// Launch Options Steam: -novid -noborder -high -threads 4 -freq 144 -refresh 144 -tickrate 128 -nojoy -nod3d9ex -noaafonts +exec autoexec.cfg +mat_vignette_enable 0 -processheap
//
// opcoes de arranque do jogo (launch options). copie e cole sem as // e altere sua resolucao e refresh rate. Uso tick 64 para poder jogar surf.
// -novid -high -w 1152 -h 864 -refresh 100 -tickrate 64 -threads 4
// -novid -high -w 1024 -h 768 -refresh 115 -tickrate 64 -threads 4 -processheap -nojoy -noforcemparms -noforcemaccel -nod3d9ex -noaafonts +mat_queue_mode 2 +mat_vignette_enable 0
// -novid -high -w 1920 -h 1080 -freq 144 -refresh 144 -tickrate 128 -threads 4 -processheap -nojoy -noforcemparms -noforcemaccel -nod3d9ex -noaafonts +mat_queue_mode 2 +mat_vignette_enable 0 +exec autoexec.cfg
//
// Last Edit 3.Set.2014

//unbindall

name "ZeroNinja ®"

// Rates
rate "128000"
cl_cmdrate "128"
cl_updaterate "128"
cl_interp "0.0"
cl_interp_ratio "1"
cl_lagcompensation "1"
 
// Mouse
sensitivity "5.8"
zoom_sensitivity_ratio_mouse "1"
m_rawinput "1"
m_pitch "0.022"
m_customaccel "0"
m_mouseaccel1 "0"
m_mouseaccel2 "0"
 
// Video
mat_setvideomode "1920 1080 1"
mat_monitorgamma "1.9" // 1.6=Brightest  2.6=Darkest
mat_queue_mode "2" // auto detect multi-core rendering
mat_vsync "0"
fps_max "145"
fps_max_menu "145"
r_dynamic "0"
r_drawtracers_firstperson "0"
mat_savechanges // write video settings to registry
 
// Audio
volume "0.55"
voice_enable "1"
voice_scale "1" // receive volume
windows_speaker_config "1" // headphone audio output
snd_musicvolume "0"
snd_mixahead "0.05" // sound delay
snd_headphone_pan_exponent "2"
snd_headphone_pan_radial_weight "2"
snd_legacy_surround "0" // emulated surround sound
snd_mute_losefocus  "1" // mute game when alt-tabbed
lobby_voice_chat_enabled "0" // voice chat in lobby
 
// HUD
hud_scaling "0.8" // CS:S sized HUD
hud_showtargetid "1"
cl_hud_background_alpha "0.100000"
cl_hud_bomb_under_radar "0"
cl_hud_color "1"
cl_hud_healthammo_style "1"
cl_hud_playercount_pos "1"
cl_hud_playercount_showcount "1"
cl_hud_radar_scale "0.900000"
cl_draw_only_deathnotices "0"
cl_righthand "1"
cl_showloadout "1"
//cl_showpos "0"
//cl_showpos 1 //se estiver 1 mostra dados no canto superior esquerdo da tela, como a velocidade do boneco.
cl_showfps "0"
net_graph "1"
net_graphproportionalfont "0" // small netgraph font
net_graphpos "1"

// Radar
cl_radar_always_centered "0"
cl_radar_rotate "1"
cl_radar_scale "0.45"
cl_radar_icon_scale_min "0.7"
cl_radar_square_with_scoreboard "0"

// Reposition gun model to mimic CS:S
viewmodel_presetpos "3" // classic
viewmodel_fov "65"
viewmodel_offset_x "2"
viewmodel_offset_y "2"
viewmodel_offset_z "-2"

// Reduce gun shifting when crouching
cl_viewmodel_shift_left_amt "0.5"
cl_viewmodel_shift_right_amt "0.5"

// Reduce gun and scope shifting/bobbing when moving
cl_bobcycle "2" // 0.98 is enforced by ESEA/ESL
cl_bob_lower_amt "5"
cl_bobamt_lat "0.1"
cl_bobamt_vert "0.1"
 
// Crosshair
cl_crosshairstyle "4"
cl_crosshairsize "2"
cl_crosshairthickness "0.5"
cl_crosshairgap "-1" // classic
cl_fixedcrosshairgap "3" // new
cl_crosshairdot "0"
cl_crosshairusealpha "1"
cl_crosshairalpha "999"
cl_crosshair_drawoutline "1"
cl_crosshair_outlinethickness "1"
cl_crosshairgap_useweaponvalue "0"
// White crosshair
cl_crosshaircolor "5"
cl_crosshaircolor_r "255"
cl_crosshaircolor_g "255"
cl_crosshaircolor_b "255"
// Debug accuracy (sv_cheats)
weapon_debug_spread_show "0" // show possible shot accuracy 
weapon_debug_spread_gap "0.67"
 
// Misc
developer "0"
con_enable "1"
con_filter_enable "2" // print console on screen
con_filter_text "Damage " // highlight damage in console
ui_steam_overlay_notification_position "bottomright"
player_nevershow_communityservermessage "1"
mm_dedicated_search_maxping "70" // max ping for matchmaking games
mm_session_search_ping_limit "70"
mm_dedicated_force_servers ""
gameinstructor_enable "0"
option_duck_method "0"
option_speed_method "0"
cl_forcepreload "1"
cl_downloadfilter "mapsonly"
cl_disablehtmlmotd "1"
cl_autohelp "1"
cl_showhelp "0"
cl_disablefreezecam "1"
cl_dm_buyrandomweapons "0"
cl_teammate_colors_show "1"
cl_autowepswitch "0" // auto weapon switch on pickup
cl_use_opens_buy_menu "0" // E openeing buy menu
cl_scoreboard_mouse_enable_binding "showmouse" // enable mouse on the scoreboard
closeonbuy "1"
hud_takesshots "0" // scoreboard screenshot at end of match
cl_clanid "6378373"
password ""

// Binds
unbind y
unbind u
unbind k
unbind alt
bind enter "messagemode"
bind \ "messagemode2"
bind v "+voicerecord"
bind "TAB" "+ng"
bind space "+jump"
bind w "+forward"
bind a "+moveleft"
bind s "+back"
bind d "+moveright"
bind MWHEELDOWN "invnext"
bind MWHEELUP "invprev"
bind home "spectate"
bind mouse1 "+attack"
bind mouse2 "+attack2"
bind mouse3 "bhopon" // toggle scroll wheel bhop
bind mouse4 "use weapon_smokegrenade"
bind mouse5 "use weapon_flashbang"
bind del "exec autoexec"
bind shift "+speed" // default
bind f "+lookatweapon" // default
bind g "drop;say_team Dropei ai. :P" // default
bind h "bot_place" // places bot for practice
bind n "+jumpthrow" // consistent smoke jump throws
bind - "toggle voice_scale 1 0" // toggle voice volume
bind = "toggle volume 0.55 0.08 0" // toggle game volume
bind "F1" "say ;noclip;say .noclip;sv_cheats 1;impulse 101;sv_showimpacts 1;sv_showimpacts_penetration 1;sv_infinite_ammo 1;sv_grenade_trajectory 1;sv_grenade_trajectory_thickness 0.5;mp_freezetime 0;mp_roundtime_defuse 60;mp_buytime 60;mp_buy_anywhere 1;bot_stop 1;mp_warmup_end;" // noclip and sv_cheats practice
bind , "showmouse"
bind . "say_team XIU POW!"
bind / "say BOM JOGO GALERA! VAMOS TENTAR JOGAR COMO ADULTOS! SEM BRIGAS! SEM OFENSAS! LEMBREM QUE ISSO E COMPETITIVO! #GOGOGO :)"
bind "F6" "go;say |Recrutamento CS:GO| www.ladykillers.tk/seja-um-tlk"
bind "F7" "go;say_team Aperta Z e elogia tudo ae time! o/ :P"
bind [ "say_team GO AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA"
bind ] "say_team GO BBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBB"
bind r "+reload"
//bind ; "say_team VEM!!!!! PRECISO DE AJUDA!!!!!"

// Aliases
alias "showmouse" // for mouse on scoreboard
alias "+ng" "+showscores; net_graph 1"
alias "-ng" "-showscores; net_graph 0"
alias bhopon "bind MWHEELDOWN +jump;bind MWHEELUP +jump;bind mouse3 bhopoff"
alias bhopoff "bind MWHEELDOWN invnext;bind MWHEELUP invprev;bind mouse3 bhopon"
alias "+jumpthrow" "+jump;-attack"
alias "-jumpthrow" "-jump"
alias mmrates "cl_interp 0.031;cl_interp_ratio 2;rate 80000" // testing rates for mm (via tesseract)

// Keypad buy binds
bind kp_ins "buy vesthelm" // 0
bind kp_del "buy vest" // .
bind kp_enter "buy defuser" // Enter
bind kp_end "buy hegrenade;give weapon_hegrenade" // 1
bind kp_downarrow "buy flashbang;give weapon_flashbang" // 2
bind kp_pgdn "buy smokegrenade;give weapon_smokegrenade" // 3
bind kp_leftarrow "buy deagle;give weapon_deagle" //4
bind kp_5 "buy incgrenade;buy molotov;give weapon_incgrenade;give weapon_molotov" // 5
bind kp_rightarrow "buy decoy;give weapon_decoy" // 6
bind kp_home "buy awp;give weapon_awp" // 7
bind kp_uparrow "buy m4a1;buy m4a4;buy ak47;give weapon_m4a1_silencer;give weapon_ak47;" // 8
bind kp_pgup "buy famas;buy galilar;give weapon_famas;give weapon_galilar" // 9
bind kp_slash "buy p90;give weapon_p90" // /
bind kp_multiply "buy ump45;give weapon_ump45" // *
bind kp_minus "buy sawedoff;buy mag7;give weapon_sawedoff;give weapon_mag7" // -
//bind kp_plus "buy p250;give weapon_p250" // +
bind kp_plus "buy tec9; buy fiveseven;" // + CZ

clear	//apaga no console o texto que estava la. apenas para melhorar a apresentacao do texto abaixo

echo "" //esta linha serve para imprimir uma linha vazia no console, apenas para melhorar a apresentacao do texto abaixo
clear
clear
echo "Suas binds de compra do teclado numerico sao:"
echo "" //alterar estas binds utilizando o f1 ate o f12 se seu teclado nao tem numpad
echo "+=====================================================+"
echo "|     NUM     |      /      |      *      |     -     |"
echo "|     PAD     |     P90     |    UMP45    | CanoCurto |"
echo "|-------------|-------------|-------------|-----------|"
echo "|      7      |      8      |      9      |     +     |"
echo "|     AWP     | M4A4 ou AK  | GALIU/FAMAS |           |"
echo "|-------------|-------------|-------------|    CZ     |"
echo "|      4      |      5      |      6      |           |"
echo "|   DESERT    |   MOLOTOV   |    DECOY    |           |"
echo "|-------------|-------------|-------------|-----------|"
echo "|      1      |      2      |      3      |   ENTER   |"
echo "| GRANADA EXP |    LIGHT    |    SMOKE    |           |"
echo "|-------------|-------------|-------------|  DEFUSE   |"
echo "|             0             |      .      |           |"
echo "|          COLETE           |   helmet    |           |"
echo "+=====================================================+"
echo ""
echo ""
//echo "+===================================================================+"
//echo "|       F1       |       F2       |       F3       |       F4       |"
//echo "|     Restart    |Mostrar Impactos|Municao infinita|  BOTs atiram   |"
//echo "|----------------|----------------|----------------|----------------|"
//echo "|       F5       |       F6       |       F7       |       F8       |"
//echo "|  Kickar BOTS   |Adicionar BOT TR|Adicionar BOT CT|  Menu de Demos |"
//echo "|----------------|----------------|----------------|----------------|"
//echo "|       F9       |      F10       |      F11       |      F12       |"
//echo "| Velocidade 50% |Velocidade 100% |Velocidade 300% |Velocidade 999% |"
//echo "+===================================================================+"
//echo ""

//bind "F1" 			"mp_restartgame 1"
//bind "F2" 			"toggle sv_showimpacts"
//bind "F3" 			"toggle sv_infinite_ammo"
//bind "F4" 			"toggle bot_dont_shoot"

//bind "f5" 			"bot_kick"
//bind "F6" 			"bot_add_t"
//bind "F7" 			"bot_add_ct"
//bind "F8" 			"demoui"

//bind "F9" 			"host_timescale 0.5;demo_timescale 0.4"
//bind "F10" 			"host_timescale 1;demo_timescale 1"
//bind "F11" 			"host_timescale 2;demo_timescale 3"
//bind "F12" 			"host_timescale 5;demo_timescale 10"

//#############################################
echo "#";echo "# ZeroNinja Autoexec.cfg carregado."
host_writeconfig // write settings to config.cfg
echo "# Config changes saved.";echo "#"
