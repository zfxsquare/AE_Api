# 开发文档
# IMemApi
使用类似`Core.Get<IMemApiSpell>()`的方法调用,可用的MemApi如下

# 职业量谱类
## 占星职业量谱 `IMemApiAstrologian` 
`DrawnCard()`

返回抽到的奥秘卡

`DrawnCrownCard()`

返回抽到的小奥秘卡

`ContainsSeal()`

返回抽到的奥秘卡是否存在相同的印(日月星)

`IsMelee()`

返回是否是近战卡

`IsRanged()`

返回是否是远程卡

`Seals()`

返回当前印的数量

`SignType()`

返回当前印的种类数量

## 诗人职业量谱 `IMemApiBard`

`ActiveSong()`

返回当前正在使用的歌曲

`Repertoire()`

返回当前诗心

`SoulVoice()`

返回当前灵魂之声

`Coda()`

返回当前尾声

## 黑魔职业量谱 IMemApiBlm

`Polyglot`

返回通晓

`UmbralStacks`

返回冰层数

`AstralStacks`

返回火层数

`StackTimer`

返回天语剩余时间

`UmbralHearts`

返回灵极心

`PolyglotTimer`

返回通宵时间

`IsParadoxReady()`

返回悖论水晶

## 舞者职业量谱

`Esprit()`

返回伶俐

`FourFoldFeathers()`

返回幻扇

`IsDancing()`

返回是否在大小舞状态

`NextStep()`

返回下一个舞步

`CompleteSteps()`

返回完成的舞步

## 黑骑职业量谱 IMemApiDarkKnight

`Blood()`

返回暗血

`DarksideTimeRemaining()`

返回暗黑剩余时间

`HasDarkArts()`

返回暗技

`ShadowTimeRemaining()`

返回弗雷时间

## 龙骑职业量谱 IMemApiDragoon

`EyeCount`

返回巨龙怒目

`FirstmindsFocusCount`

返回天龙眼

`IsLOTDActive`

返回是否在红龙状态

`LOTDTimer`

返回红龙剩余时间

## 绝枪职业量谱 IMemApiGunBreaker

`Ammo`

返回子弹

## 机工职业量谱 IMemApiMCH

`GetHeat()`

返回热量

`GetBattery()`

返回电量

`Robotactive()`

返回机器人是否在场

`OverHeated()`

返回是否在过热状态

`SummonRemain()`

返回机器人剩余时间

`OverheatRemain()`

返回过热剩余时间

## 武僧职业量谱 IMemApiMonk

`ChakraCount` 

返回查克拉

`BlitzTimer`

返回必杀技时间

`ActiveNadi`

返回必杀状态(阴阳)

`MastersGauge`

返回脉轮列表

## 忍者职业量谱 IMemApiNinja

`HutonTimer`

返回风遁时间

`Ninki`

返回忍气

## 骑士职业量谱 IMemApiPaladin

`Oath`

返回忠义

## 镰刀职业量谱 IMemApiReaper

`ShroudGauge`

返回魂衣

`SoulGauge`

返回灵魂

`VoidShroud`

返回虚无魂

`LemureShroud`

返回夜游魂

## 赤魔职业量谱 IMemApiRedMage

`WhiteMana()`

返回白魔元

`BlackMana()`

返回黑魔元

`ManaStacks()`

返回魔元集

## 贤者职业量谱 IMemApiSage

`AddersgallTimer()`

返回蛇胆时间

`Addersgall()`

返回蛇胆(蓝豆子)

`Addersting()`

返回蛇刺(红豆子)

`Eukrasia()`

返回是否处在均衡

## 武士职业量谱 IMemApiSamurai

`Kenki()`

返回剑气

`HasSetsu()`

返回是否有雪

`HasGetsu()`

返回是否有月

`HasKa()`

返回是否有花

`Sen()`

返回闪的个数

`MeditationStacks()`

返回剑压

`Kaeshi()`

返回当前回返技能

## 学者职业量谱 IMemApiScholar

`Aetherflow()`

返回以太超流

`SeraphTimer()`

返回大天使时间

`FairyGauge()`

返回异想以太

`HasPet`

返回是否有小仙女

`Dissipation()`

返回是否可用转化

## 召唤职业量谱 IMemApiSummoner

`HasAetherflowStacks`

返回是否有以太超流

`Aetherflow`

返回以太超流层数

`IsPetReady`

返回召唤兽是否可用

`ActivePetType`

返回当前召唤兽

`InBahamut`

返回龙神附体状态

`InPhoenix`

返回不死鸟附体状态

## 战士职业量谱 IMemApiWarrior

`BeastGauge`

返回兽魂

## 白魔职业量谱 IMemApiWhiteMage

`Lily()`

返回兰花数量

`BloodLily()`

返回红花数量

# 其他API

## Buff检测 IMemApiBuff

`HasAura`

返回是否有Buff

`GetAuraTimeleft`

返回Buff剩余时间

`GetStack`

返回Buff层数

`GetAuraParam`

未知属性

`HasMyAura`

返回是否存在自己赋予的buff

`HasAnyAura`

返回是否存在列表中的任意buff

`GetBuffCount`

返回Buff数量

`BuffList`

返回Buff列表

`HasCanDispel`

返回Buff是否可被驱散

## 聊天相关 IMemApiChatMessage

`PrintChat`

打印文本

`Say` `Shout` 等等频道

在对应频道说话

## 自身状态相关 IMemApiCondition

`IsBoundByDuty()`

返回在任务中

`IsInCombat()`

返回在战斗中

`IsInCutsceneOrQuestEvent()`

返回过场动画或任务动画中

`IsBetweenAreas()`

返回过图中

## 倒计时相关 IMemApiCountdown

`IsActive()`

返回是否在倒计时

`TimeRemaining()`

返回倒计时剩余时间

## 头标地标相关 IMemApiMaker

`GetMarkerByObject()`

返回obj的头标

`GetCharacterByMarker()`

返回有头标的chara

`WayMarker`

返回地标状态

## 地图相关 IMemApiMap

`GetCurrTerrId()`

返回当前场地id

`ZoneName`

返回当前地图名称

## 移动相关 IMemApiMove

`IsMoving()`

返回是否在移动

`GetPos()`

返回坐标

`GetRot()`

返回角度

## 队伍相关 IMemApiParty

`GetParty()`

返回当前小队,按小队列表排序

## 发送指令相关 IMemApiSendMessage

`SendMessage()`

发送指令

# Helper

## BossAOE技能 Bossaoelist 

`list`

返回BossAOE技能的数组

## 死刑技能 DeathSentencelist

`list`

返回死刑技能的数组

## 小队 PartyHelper

`InParty`

返回是否在小队中

`NumMembers`

返回小队人数

`GetAnotherTank`

返回另一个T

`DeadAllies`

返回死亡列表

`CastableTanks`

返回坦克列表

`CastableHealers`

返回治疗列表

`CastableMainTanks`

返回开盾T

`CastableAlliesWithin3` `CastableAlliesWithin15` 等

返回指定范围内的队友

## 目标 TargetHelper

`IsBoss`

返回目标是否为BOSS

`GetTargetDistanceTest`

返回目标距离

`GetNearbyEnemyCount`

返回自身周围敌人数量

`GetEnemyCountInsideSector`

返回扇形内敌人数量

`GetEnemyCountInsideRect`

返回矩形内敌人数量

`TargercastingIsbossaoe`

返回目标是否在释放AOE

## 天气 WeatherHelper

`GetWeatherId()`

返回当前天气

## 常用API

`AI.Instance.BattleData.CurrBattleTimeInMs`

当前战斗时间

`Core.Get<IMemApiSpell>().GetLastComboSpellId()`

上一个连击技能

`SettingMgr.GetSetting<GeneralSettings>().AttackRange`

设置的近战范围

