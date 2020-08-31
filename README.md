### 1、更改比分接口

```
{
		//比赛id
    "gameId":1,
		//第几局比赛
    "gameNumber":1,
    //更改比分之后主队分数
    "homeTeamScore":1,
		//更改比分之后客队分数
    "visitingTeamScore":1,
    //操作类型 0：正常加分 1：比赛开始  2:比赛结束 3:比赛得分 7:中场休息 8:球队弃权 9:撤销上一步
    "operationType":0,
    //比赛弃权类型 默认为0:正常结束本局 1：本局弃权 2：本场弃权
    "overType":0,
    //弃权队伍   默认为0：正常结束传0  1：主队 2：客队
    "waiverTeam":0
}
```



### 2、比赛列表接口

```
[
    {
    		//比赛id
        "gameId":1,
        "gameName":"赛事名称",
        "gameImg":"赛事图片",
				//比赛类型 1：几局几胜制(比如3局2胜) 2：要把所有的都打完
				"gameFormatType":1,
				//主队信息
        "homeTeam":{
            "teamName":"主队名称",
            "teamImg":"主队队徽图片",
            //队伍id
            "teamId":1
        },
        //客队信息
        "visitingTeam":{
            "teamName":"客队名称",
            "teamImg":"客队队徽图片",
            "teamId":2
        },
        //对局数组
        "gameList":[
            {
            		//主队队员id
                "homePlayerId":1,
                "homePlayerName":"本局主队队员名称",
                //主队队员性别  0:男 1:女
                "homePlayerSex":1,
                "homePlayerImg":"本局主队队员头像",
                "visitingPlayerId":2,
                "visitingPlayerName":"本局客队队员名称",
                "visitingPlayerSex":2,
                "visitingPlayerImg":"本局客队队员头像",
                //本局比赛类型 0:男单 1：女单  2：男双 3：女双 4：混双
                "gameDetailsType":0
            },
            {
                "homePlayerId":3,
                "homePlayerName":"本局主队队员名称",
                "homePlayerSex":1,
                "homePlayerImg":"本局主队队员头像",
                "visitingPlayerId":4,
                "visitingPlayerName":"本局客队队员名称",
                "visitingPlayerSex":2,
                "visitingPlayerImg":"本局客队队员头像",
                "gameDetailsType":0
            },
            {
                "homePlayerId":5,
                "homePlayerName":"本局主队队员名称",
                "homePlayerSex":1,
                "homePlayerImg":"本局主队队员头像",
                "visitingPlayerId":6,
                "visitingPlayerName":"本局客队队员名称",
                "visitingPlayerSex":2,
                "visitingPlayerImg":"本局客队队员头像",
                "gameDetailsType":0
            }
        ]
    },
    Object{...}
]
```


