# serverevents
- server_spawn
    - 说明：服务器启动时触发此事件
    - hostname <kbd>string</kbd> __服务器名称__
    - address <kbd>string</kbd> __主机名, IP 或者 DNS名称__
    - port <kbd>short</kbd> __服务器端口__
    - game <kbd>string</kbd> __游戏名__
    - mapname <kbd>string</kbd> __地图名称__
    - maxplayers <kbd>long</kbd> __最大玩家数__
    - os <kbd>string</kbd> __服务器系统(WIN32, LINUX)__
    - dedicated <kbd>bool</kbd> __是否为专用服务器__
    - official <kbd>bool</kbd> __是否为Valve官方专用服务器__
    - password <kbd>bool</kbd> __是否设置密码__
- server_pre_shutdown
    - 说明：服务器即将关闭时触发此事件
    - reason <kbd>string</kbd> __服务器即将关闭的原因__
- server_shutdown
    - 说明：服务器关闭时触发此事件
    - reason <kbd>string</kbd> __服务器关闭的原因__
- server_cvar
    - 说明：服务器的cvar发生改变时触发此事件
    - cvarname <kbd>string</kbd> __cvar名称, 如"mp_roundtime"__
    - cvarvalue <kbd>string</kbd> __新的cvar值__
- server_message
    - 说明：通用服务器信息
    - text <kbd>string</kbd> __信息内容__
- server_addban
    - 说明：服务器中有玩家被封禁时触发此事件
    - name <kbd>string</kbd> __玩家名__
    - userid <kbd>short</kbd> __在服务器中的userid__
    - networkid <kbd>string</kbd> __玩家网络ID__
    - ip <kbd>string</kbd> __玩家IP__
    - duration <kbd>string</kbd> __封禁时间__
    - by <kbd>string</kbd> __封禁者__
    - kicked <kbd>bool</kbd> __玩家是否同时被踢出服务器__
- player_info
    - 说明：玩家名字更改时触发此事件
    - name <kbd>string</kbd> __玩家名__
    - index <kbd>byte</kbd> __玩家slot (实体index -1)__
    - userid <kbd>short</kbd> __玩家在服务器上的userid__
    - networkid <kbd>string</kbd> __玩家网络ID__
    - bot <kbd>bool</kbd> __是否为bot__
