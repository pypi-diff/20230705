# Comparing `tmp/fgo_api_types-2023.6.8.15.39.7.tar.gz` & `tmp/fgo_api_types-2023.7.5.6.44.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.6.8.15.39.7.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.7.5.6.44.7.tar", max compression
```

## Comparing `fgo_api_types-2023.6.8.15.39.7.tar` & `fgo_api_types-2023.7.5.6.44.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-06-08 15:38:35.602324 fgo_api_types-2023.6.8.15.39.7/LICENSE
--rw-r--r--   0        0        0      449 2023-06-08 15:38:35.602324 fgo_api_types-2023.6.8.15.39.7/README.md
--rw-r--r--   0        0        0        0 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/common.py
--rw-r--r--   0        0        0    38038 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/enums.py
--rw-r--r--   0        0        0   158848 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    76474 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/nice.py
--rw-r--r--   0        0        0    50915 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18670 2023-06-08 15:39:07.010581 fgo_api_types-2023.6.8.15.39.7/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-06-08 15:39:07.426585 fgo_api_types-2023.6.8.15.39.7/pyproject.toml
--rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 fgo_api_types-2023.6.8.15.39.7/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-05 06:43:48.212693 fgo_api_types-2023.7.5.6.44.7/LICENSE
+-rw-r--r--   0        0        0      449 2023-07-05 06:43:48.212693 fgo_api_types-2023.7.5.6.44.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 06:44:07.492961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-07-05 06:44:07.492961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-07-05 06:44:07.492961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/common.py
+-rw-r--r--   0        0        0    38038 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   160313 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    78308 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    53003 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    19183 2023-07-05 06:44:07.496961 fgo_api_types-2023.7.5.6.44.7/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-07-05 06:44:07.836966 fgo_api_types-2023.7.5.6.44.7/pyproject.toml
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 fgo_api_types-2023.7.5.6.44.7/PKG-INFO
```

### Comparing `fgo_api_types-2023.6.8.15.39.7/LICENSE` & `fgo_api_types-2023.7.5.6.44.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/basic.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/common.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/enums.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/gameenums.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/gameenums.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,14 +203,15 @@
     BUDDY_POINT_UP = 129
     ADD_FIELD_CHANGE_TO_FIELD = 130
     SUB_FIELD_BUFF = 131
     EVENT_FORTIFICATION_POINT_UP = 132
     GAIN_NP_INDIVIDUAL_SUM = 133
     SET_QUEST_ROUTE_FLAG = 134
     LAST_USE_PLAYER_SKILL_COPY = 135
+    CHANGE_ENEMY_MASTER_FACE = 136
 
 
 class NiceFuncType(StrEnum):
     """Function Type Enum"""
 
     none = "none"
     addState = "addState"
@@ -307,14 +308,15 @@
     buddyPointUp = "buddyPointUp"
     addFieldChangeToField = "addFieldChangeToField"
     subFieldBuff = "subFieldBuff"
     eventFortificationPointUp = "eventFortificationPointUp"
     gainNpIndividualSum = "gainNpIndividualSum"
     setQuestRouteFlag = "setQuestRouteFlag"
     lastUsePlayerSkillCopy = "lastUsePlayerSkillCopy"
+    changeEnemyMasterFace = "changeEnemyMasterFace"
 
 
 FUNC_TYPE_NAME: dict[int, NiceFuncType] = {
     0: NiceFuncType.none,
     1: NiceFuncType.addState,
     2: NiceFuncType.subState,
     3: NiceFuncType.damage,
@@ -409,14 +411,15 @@
     129: NiceFuncType.buddyPointUp,
     130: NiceFuncType.addFieldChangeToField,
     131: NiceFuncType.subFieldBuff,
     132: NiceFuncType.eventFortificationPointUp,
     133: NiceFuncType.gainNpIndividualSum,
     134: NiceFuncType.setQuestRouteFlag,
     135: NiceFuncType.lastUsePlayerSkillCopy,
+    136: NiceFuncType.changeEnemyMasterFace,
 }
 
 
 class FuncTargetType(IntEnum):
     SELF = 0
     PT_ONE = 1
     PT_ANOTHER = 2
@@ -1728,14 +1731,15 @@
     QUEST_REWARD_ICON = 8
     COSTUME_RELEASE = 9
     COSTUME_GET = 10
     COMMAND_CODE = 11
     EVENT_POINT_BUFF = 12
     EVENT_BOARD_GAME_TOKEN = 13
     EVENT_COMMAND_ASSIST = 14
+    EVENT_HEEL_PORTRAIT = 15
 
 
 class NiceGiftType(StrEnum):
     """Gift Type Enum"""
 
     servant = "servant"
     item = "item"
@@ -1747,14 +1751,15 @@
     questRewardIcon = "questRewardIcon"
     costumeRelease = "costumeRelease"
     costumeGet = "costumeGet"
     commandCode = "commandCode"
     eventPointBuff = "eventPointBuff"
     eventBoardGameToken = "eventBoardGameToken"
     eventCommandAssist = "eventCommandAssist"
+    eventHeelPortrait = "eventHeelPortrait"
 
 
 GIFT_TYPE_NAME: dict[int, NiceGiftType] = {
     1: NiceGiftType.servant,
     2: NiceGiftType.item,
     3: NiceGiftType.friendship,
     4: NiceGiftType.userExp,
@@ -1764,14 +1769,15 @@
     8: NiceGiftType.questRewardIcon,
     9: NiceGiftType.costumeRelease,
     10: NiceGiftType.costumeGet,
     11: NiceGiftType.commandCode,
     12: NiceGiftType.eventPointBuff,
     13: NiceGiftType.eventBoardGameToken,
     14: NiceGiftType.eventCommandAssist,
+    15: NiceGiftType.eventHeelPortrait,
 }
 
 
 class ShopType(IntEnum):
     NONE = 0
     EVENT_ITEM = 1
     MANA = 2
@@ -2180,14 +2186,16 @@
     SVT_FRIENDSHIP_CLASS_NUM_ABOVE = 178
     NOT_WAR_CLEAR = 179
     SVT_SKILL_LV_CLASS_NUM_ABOVE = 180
     SVT_CLASS_LV_UP_COUNT = 181
     SVT_CLASS_SKILL_LV_UP_COUNT = 182
     SVT_CLASS_LIMIT_UP_COUNT = 183
     SVT_CLASS_FRIENDSHIP_COUNT = 184
+    COMPLETE_HEEL_PORTRAIT = 185
+    NOT_COMPLETE_HEEL_PORTRAIT = 186
 
 
 class NiceCondType(StrEnum):
     """Condition Type Enum"""
 
     none = "none"
     questClear = "questClear"
@@ -2367,14 +2375,16 @@
     svtFriendshipClassNumAbove = "svtFriendshipClassNumAbove"
     notWarClear = "notWarClear"
     svtSkillLvClassNumAbove = "svtSkillLvClassNumAbove"
     svtClassLvUpCount = "svtClassLvUpCount"
     svtClassSkillLvUpCount = "svtClassSkillLvUpCount"
     svtClassLimitUpCount = "svtClassLimitUpCount"
     svtClassFriendshipCount = "svtClassFriendshipCount"
+    completeHeelPortrait = "completeHeelPortrait"
+    notCompleteHeelPortrait = "notCompleteHeelPortrait"
 
 
 COND_TYPE_NAME: dict[int, NiceCondType] = {
     0: NiceCondType.none,
     1: NiceCondType.questClear,
     2: NiceCondType.itemGet,
     3: NiceCondType.useItemEternity,
@@ -2552,14 +2562,16 @@
     178: NiceCondType.svtFriendshipClassNumAbove,
     179: NiceCondType.notWarClear,
     180: NiceCondType.svtSkillLvClassNumAbove,
     181: NiceCondType.svtClassLvUpCount,
     182: NiceCondType.svtClassSkillLvUpCount,
     183: NiceCondType.svtClassLimitUpCount,
     184: NiceCondType.svtClassFriendshipCount,
+    185: NiceCondType.completeHeelPortrait,
+    186: NiceCondType.notCompleteHeelPortrait,
 }
 
 
 class VoiceCondType(IntEnum):
     BIRTH_DAY = 1
     EVENT = 2
     FRIENDSHIP = 3
@@ -3894,14 +3906,15 @@
     RESURRECTION = 42
     PLAY_MOTION = 71
     MESSAGE = 72
     MESSAGE_GROUP = 73
     NOBLE_PHANTASM = 80
     BATTLE_END = 90
     LOSE_END = 91
+    BATTLE_END_NOT_RELATED_SURVIVAL_STATUS = 92
     CHANGE_THINKING = 99
 
 
 class NiceAiActType(StrEnum):
     """AI Act Type Enum"""
 
     none = "none"
@@ -3923,14 +3936,15 @@
     resurrection = "resurrection"
     playMotion = "playMotion"
     message = "message"
     messageGroup = "messageGroup"
     noblePhantasm = "noblePhantasm"
     battleEnd = "battleEnd"
     loseEnd = "loseEnd"
+    battleEndNotRelatedSurvivalStatus = "battleEndNotRelatedSurvivalStatus"
     changeThinking = "changeThinking"
 
 
 AI_ACT_TYPE_NAME: dict[int, NiceAiActType] = {
     0: NiceAiActType.none,
     1: NiceAiActType.random,
     2: NiceAiActType.attack,
@@ -3950,14 +3964,15 @@
     42: NiceAiActType.resurrection,
     71: NiceAiActType.playMotion,
     72: NiceAiActType.message,
     73: NiceAiActType.messageGroup,
     80: NiceAiActType.noblePhantasm,
     90: NiceAiActType.battleEnd,
     91: NiceAiActType.loseEnd,
+    92: NiceAiActType.battleEndNotRelatedSurvivalStatus,
     99: NiceAiActType.changeThinking,
 }
 
 
 class AiActTarget(IntEnum):
     NONE = 0
     RANDOM = 1
@@ -5012,7 +5027,46 @@
     16: NiceNpcServantFollowerFlag.applySvtChange,
     32: NiceNpcServantFollowerFlag.hideEquip,
     64: NiceNpcServantFollowerFlag.noDisplayBonusIconEquip,
     256: NiceNpcServantFollowerFlag.hideTreasureDeviceLv,
     512: NiceNpcServantFollowerFlag.hideTreasureDeviceDetail,
     1024: NiceNpcServantFollowerFlag.hideRarity,
 }
+
+
+class ClassBoardSquareFlag(IntEnum):
+    START = 1
+    BLANK = 2
+
+
+class NiceClassBoardSquareFlag(StrEnum):
+    """Class Board Square Flag"""
+
+    start = "start"
+    blank = "blank"
+
+
+CLASS_BOARD_SQUARE_FLAG_NAME: dict[int, NiceClassBoardSquareFlag] = {
+    1: NiceClassBoardSquareFlag.start,
+    2: NiceClassBoardSquareFlag.blank,
+}
+
+
+class ClassBoardSkillType(IntEnum):
+    NONE = 0
+    PASSIVE = 1
+    COMMAND_SPELL = 2
+
+
+class NiceClassBoardSkillType(StrEnum):
+    """Class Board Skill Type"""
+
+    none = "none"
+    passive = "passive"
+    commandSpell = "commandSpell"
+
+
+CLASS_BOARD_SKILL_TYPE_NAME: dict[int, NiceClassBoardSkillType] = {
+    0: NiceClassBoardSkillType.none,
+    1: NiceClassBoardSkillType.passive,
+    2: NiceClassBoardSkillType.commandSpell,
+}
```

### Comparing `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/nice.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/nice.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 from .gameenums import (
     NiceAiActNum,
     NiceAiActTarget,
     NiceAiActType,
     NiceAiCond,
     NiceBuffType,
     NiceCardType,
+    NiceClassBoardSkillType,
+    NiceClassBoardSquareFlag,
     NiceCombineAdjustTarget,
     NiceCommandCardAttackType,
     NiceCommonConsumeType,
     NiceCondType,
     NiceConsumeType,
     NiceEventCombineCalc,
     NiceEventFortificationSvtType,
@@ -164,14 +166,16 @@
     script = "{base_url}/{region}/Script/{script_path}.txt"
     bgmLogo = "{base_url}/{region}/MyRoomSound/soundlogo_{logo_id:0>3}.png"
     servantModel = "{base_url}/{region}/Servants/{item_id}/manifest.json"
     movie = "{base_url}/{region}/Movie/{item_id}.mp4"
     commandSpell = "{base_url}/{region}/CommandSpell/cs_{item_id:0>4}.png"
     enemyMasterFace = "{base_url}/{region}/EnemyMasterFace/enemyMstFace{item_id}.png"
     enemyMasterFigure = "{base_url}/{region}/EnemyMasterFigure/figure{item_id}.png"
+    classBoardIcon = "{base_url}/{region}/ClassBoard/Icon/{item_id}.png"
+    classBoardBg = "{base_url}/{region}/ClassBoard/Bg/{item_id}.png"
 
 
 COSTUME_LIMIT_NO_LESS_THAN = 11
 LIMIT_TO_FACE_ID = {0: 0, 1: 1, 2: 1, 3: 2, 4: 3}
 LIMIT_TO_FIGURE_ID = {0: 0, 1: 1, 2: 1, 3: 2, 4: 2}
 
 
@@ -638,28 +642,28 @@
     eventId: int  # 0,
     flag: int  # 0
     releaseConditions: list[NiceSvtSkillRelease]
 
 
 class NiceSkill(BaseModelORJson):
     id: int
-    num: int = -1
+    num: int = 0
     name: str
     originalName: str
     ruby: str
     detail: Optional[str] = None
     unmodifiedDetail: Optional[str] = None
     type: NiceSkillType
     svtId: int
-    strengthStatus: int = -1
-    priority: int = -1
-    condQuestId: int = -1
-    condQuestPhase: int = -1
-    condLv: int = -1
-    condLimitCount: int = -1
+    strengthStatus: int = 0
+    priority: int = 0
+    condQuestId: int = 0
+    condQuestPhase: int = 0
+    condLv: int = 0
+    condLimitCount: int = 0
     icon: Optional[HttpUrl] = None
     coolDown: list[int]
     actIndividuality: list[NiceTrait]
     script: NiceSkillScript
     extraPassive: list[ExtraPassive]
     skillAdd: list[NiceSkillAdd]
     skillSvts: list[NiceSkillSvt] = []
@@ -676,14 +680,15 @@
     defence: list[int]
     np: list[int]
 
 
 class NiceTdSvt(BaseModelORJson):
     svtId: int
     num: int
+    npNum: int
     priority: int
     damage: list[int]
     strengthStatus: int
     flag: int
     imageIndex: int
     condQuestId: int
     condQuestPhase: int
@@ -693,14 +698,15 @@
     card: NiceCardType
     releaseConditions: list[NiceSvtSkillRelease] = []
 
 
 class NiceTd(BaseModelORJson):
     id: int
     num: int
+    npNum: int
     card: NiceCardType
     name: str
     originalName: str
     ruby: str
     icon: Optional[HttpUrl] = None
     rank: str
     type: str
@@ -1996,14 +2002,27 @@
 class NiceQuestRelease(BaseModelORJson):
     type: NiceCondType
     targetId: int
     value: int
     closedMessage: str
 
 
+class NiceQuestReleaseOverwrite(BaseModelORJson):
+    priority: int
+    # imagePriority: int
+    condType: NiceCondType
+    condId: int
+    condNum: int
+    closedMessage: str
+    overlayClosedMessage: str
+    eventId: int
+    startedAt: int
+    endedAt: int
+
+
 class NiceQuestPhaseScript(BaseModelORJson):
     phase: int
     scripts: list[ScriptLink]
 
 
 class NiceQuest(BaseModelORJson):
     id: int
@@ -2021,14 +2040,15 @@
     warLongName: str
     chapterId: int
     chapterSubId: int
     chapterSubStr: str
     giftIcon: HttpUrl | None = None
     gifts: list[NiceGift]
     releaseConditions: list[NiceQuestRelease]
+    releaseOverwrites: list[NiceQuestReleaseOverwrite]
     phases: list[int]
     phasesWithEnemies: list[int] = Field(
         [],
         title="List of phases with enemies data from Rayshift",
         description="List of phases with enemies data from Rayshift.",
     )
     phasesNoBattle: list[int] = Field(
@@ -2571,7 +2591,67 @@
     timingDescription: Optional[AiTiming] = None
 
 
 class NiceAiCollection(BaseModelORJson):
     mainAis: list[NiceAi]
     relatedAis: list[NiceAi]
     relatedQuests: list[StageLink]
+
+
+class NiceClassBoardClass(BaseModelORJson):
+    classId: int
+    className: SvtClass
+    condType: NiceCondType
+    condTargetId: int
+    condNum: int
+
+
+class NiceClassBoardCommandSpell(BaseModelORJson):
+    id: int
+    commandSpellId: int
+    name: str
+    detail: str
+    functions: list[NiceFunction]
+
+
+class NiceClassBoardLock(BaseModelORJson):
+    id: int
+    items: list[NiceItemAmount]
+    closedMessage: str
+    condType: NiceCondType
+    condTargetId: int
+    condNum: int
+
+
+class NiceClassBoardSquare(BaseModelORJson):
+    id: int
+    icon: HttpUrl | None
+    items: list[NiceItemAmount]
+    posX: int
+    posY: int
+    skillType: NiceClassBoardSkillType
+    targetSkill: NiceSkill | None
+    upSkillLv: int
+    targetCommandSpell: NiceClassBoardCommandSpell | None
+    lock: NiceClassBoardLock | None
+    flags: list[NiceClassBoardSquareFlag]
+    priority: int
+
+
+class NiceClassBoardLine(BaseModelORJson):
+    id: int
+    prevSquareId: int
+    nextSquareId: int
+
+
+class NiceClassBoard(BaseModelORJson):
+    id: int
+    name: str
+    icon: HttpUrl
+    dispItems: list[NiceItem]
+    closedMessage: str
+    condType: NiceCondType
+    condTargetId: int
+    condNum: int
+    classes: list[NiceClassBoardClass]
+    squares: list[NiceClassBoardSquare]
+    lines: list[NiceClassBoardLine]
```

### Comparing `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/raw.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/raw.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,15 @@
     detail: str  # "Deal heavy damage to all enemies [{0}] + restore your NP Gauge <effect increases with Overcharge>",
     detailShort: str  # "Deal heavy damage to all enemies [{0}] + restore your NP Gauge <effect increases with Overcharge>"
 
 
 class MstSvtTreasureDevice(BaseModelORJson):
     damage: list[int]  # [5, 11, 17, 11, 23, 33],
     strengthStatus: int  # 1,
+    treasureDeviceNum: int | None = 1
     svtId: int  # 400900,
     num: int  # 1,
     priority: int  # 101,
     flag: int  # 0,
     imageIndex: int  # 0,
     treasureDeviceId: int  # 400901,
     condQuestId: int  # 0,
@@ -1617,14 +1618,28 @@
     targetId: int  # 100100
     value: int  # 4
     openLimit: int = 0  # 0
     closedMessageId: int  # 2
     imagePriority: int  # 3000
 
 
+class MstQuestReleaseOverwrite(BaseModelORJson):
+    questId: int
+    priority: int
+    imagePriority: int
+    condType: int
+    condId: int
+    condNum: int
+    closedMessageId: int
+    overlayClosedMessage: str
+    eventId: int
+    startedAt: int
+    endedAt: int
+
+
 class MstQuestConsumeItem(BaseModelORJson):
     itemIds: list[int]  # [94032205, 94032206]
     nums: list[int]  # [160, 220]
     questId: int  # 94032410
 
 
 class MstClosedMessage(BaseModelORJson):
@@ -1926,14 +1941,15 @@
     snippets: list[str]
 
 
 class QuestEntity(BaseModelORJson):
     mstQuest: MstQuest
     mstQuestConsumeItem: list[MstQuestConsumeItem]
     mstQuestRelease: list[MstQuestRelease]
+    mstQuestReleaseOverwrite: list[MstQuestReleaseOverwrite]
     mstClosedMessage: list[MstClosedMessage]
     mstGift: list[MstGift]
     mstGiftAdd: list[MstGiftAdd]
     mstItem: list[MstItem] = []
     phases: list[int]
     phasesWithEnemies: list[int] = []
     phasesNoBattle: list[int] = []
@@ -2071,14 +2087,97 @@
 
 class AiCollection(BaseModelORJson):
     mainAis: list[AiEntity]
     relatedAis: list[AiEntity]
     relatedQuests: list[StageLink]
 
 
+class MstClassBoardBase(BaseModelORJson):
+    dispItemIds: list[int]
+    id: int
+    name: str
+    iconId: int
+    closedMessage: str
+    condType: int
+    condTargetId: int
+    condNum: int
+
+
+class MstClassBoardClass(BaseModelORJson):
+    classBoardBaseId: int
+    classId: int
+    condType: int
+    condTargetId: int
+    condNum: int
+
+
+class MstClassBoardCommandSpell(BaseModelORJson):
+    funcIds: list[int]
+    expandedFuncId: list[FunctionEntityNoReverse] = []
+    svals: list[str]
+    id: int
+    commandSpellId: int
+    lv: int
+    name: str
+    detail: str
+    vals: str
+
+
+class MstClassBoardLine(BaseModelORJson):
+    classBoardBaseId: int
+    id: int
+    prevSquareId: int
+    nextSquareId: int
+
+
+class MstClassBoardLock(BaseModelORJson):
+    itemIds: list[int]
+    itemNums: list[int]
+    id: int
+    closedMessage: str
+    condType: int
+    condTargetId: int
+    condNum: int
+
+
+class MstClassBoardSquare(BaseModelORJson):
+    itemIds: list[int]
+    itemNums: list[int]
+    classBoardBaseId: int
+    id: int
+    iconId: int
+    posX: int
+    posY: int
+    skillType: int
+    targetId: int
+    upSkillLv: int
+    lockId: int
+    assetId: int
+    flag: int
+    priority: int
+
+
+class MstFuncDisp(BaseModelORJson):
+    funcIds: list[int]
+    id: int
+    detail: str
+
+
+class ClassBoardEntity(BaseModelORJson):
+    mstClassBoardBase: MstClassBoardBase
+    mstClassBoardClass: list[MstClassBoardClass]
+    mstClassBoardLine: list[MstClassBoardLine]
+    mstClassBoardSquare: list[MstClassBoardSquare]
+    mstClassBoardLock: list[MstClassBoardLock]
+    mstClassBoardCommandSpell: list[MstClassBoardCommandSpell]
+    mstItem: list[MstItem]
+    mstSkill: list[SkillEntityNoReverse]
+    # mstFuncDisp: list[MstFuncDisp]
+
+
 class AssetStorageLine(BaseModelORJson):
     first: str = Field(
         ...,
         title="First field",
         description="Unused in JP/NA/KR. Download name of the asset in CN/TW.",
     )
     required: str = Field(
```

### Comparing `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/rayshift.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.6.8.15.39.7/fgo_api_types/search.py` & `fgo_api_types-2023.7.5.6.44.7/fgo_api_types/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     rarity: list[int] = Query([])
     className: list[SvtClass] = Query(PLAYABLE_CLASS_LIST)
     gender: list[NiceGender] = Query([])
     attribute: list[Attribute] = Query([])
     trait: list[Union[Trait, int]] = Query([])
     notTrait: list[Union[Trait, int]] = Query([])
     voiceCondSvt: list[int] = Query([])
+    profileContains: str | None = Query(None, max_length=999)
 
     def hasSearchParams(self) -> bool:
         return any(
             [
                 self.name,
                 self.illustrator,
                 self.cv,
@@ -60,14 +61,15 @@
                 self.rarity,
                 self.className != PLAYABLE_CLASS_LIST,
                 self.gender,
                 self.attribute,
                 self.trait,
                 self.notTrait,
                 self.voiceCondSvt,
+                self.profileContains,
             ]
         )
 
     DESCRIPTION: ClassVar[str] = inspect.cleandoc(
         """
         Search and return the list of matched servant entities.
 
@@ -82,14 +84,15 @@
         - **gender**: `female`, `male` or `unknown`.
         - **attribute**: `human`, `sky`, `earth`, `star` or `beast`.
         - **trait**: an integer or an item in the `trait` enum. See the traits detail in the Nice Servant response.
         - **notTrait**: an integer or an item in the `trait` enum. The result entities won't have any of the traits
         in the list.
         - **voiceCondValue**: servant `collectionNo` or servant `ID`. Will find the servants that
         have voice lines directed to the given servants.
+        - **profileContains**: string. Will search the servant's profile comments for the string.
 
         At least one of `name`, `type`, `rarity`, `className`, `gender`, `attribute`,
         `trait` or `voiceCondSvt` is required for the query.
         """
     )
 
 
@@ -105,14 +108,15 @@
     rarity: list[int] = Query([], ge=0, le=5)
     className: list[SvtClass] = Query([])
     gender: list[NiceGender] = Query([])
     attribute: list[Attribute] = Query([])
     trait: list[Union[Trait, int]] = Query([])
     notTrait: list[Union[Trait, int]] = Query([])
     voiceCondSvt: list[int] = Query([])
+    profileContains: str | None = Query(None, max_length=999)
 
     def hasSearchParams(self) -> bool:
         return any(
             [
                 self.name,
                 self.illustrator,
                 self.cv,
@@ -121,14 +125,15 @@
                 self.rarity,
                 self.className,
                 self.gender,
                 self.attribute,
                 self.trait,
                 self.notTrait,
                 self.voiceCondSvt,
+                self.profileContains,
             ]
         )
 
     DESCRIPTION: ClassVar[str] = inspect.cleandoc(
         """
         Search and return the list of matched servant entities.
 
@@ -143,14 +148,15 @@
         - **gender**: `female`, `male` or `unknown`.
         - **attribute**: `human`, `sky`, `earth`, `star` or `beast`.
         - **trait**: an integer or an item in the `trait` enum. See the traits detail in the Nice Servant response.
         - **notTrait**: an integer or an item in the `trait` enum. The result entities won't have any of the traits
         in the list.
         - **voiceCondValue**: servant `collectionNo` or servant `ID`. Will find the servants that
         have voice lines directed to the given servants.
+        - **profileContains**: string. Will search the servant's profile comments for the string.
 
         At least one of `name`, `type`, `rarity`, `className`, `gender`, `attribute`
         `trait` or `voiceCondSvt` is required for the query.
         """
     )
 
 
@@ -477,24 +483,26 @@
 
 
 @dataclass
 class ScriptSearchQueryParams:
     region: Region
     query: str = Query(..., max_length=999)
     scriptFileName: str | None = Query(default=None, max_length=99)
+    rawScript: bool | None = Query(default=None)
     warId: list[int] = Query([])
     limit: int | None = Query(None, le=500)
 
     DESCRIPTION: ClassVar[str] = inspect.cleandoc(
         """
         Search and return the list of matching scripts.
 
         - **query**: search query https://groonga.org/docs/reference/grn_expr/query_syntax.html.
         (Queries starting with `column:` are not supported).
         - **scriptFileName**: The script name should contain this string.
+        - **rawScript**: Search raw script instead of only dialogue
         - **warId**: War ID of the quest that with the script.
         For example: 30001 string for LB1 scripts or 9401 for interlude scripts.
         """
     )
 
     def hasSearchParams(self) -> bool:
         return 1 <= len(self.query.strip()) <= 999
```

### Comparing `fgo_api_types-2023.6.8.15.39.7/pyproject.toml` & `fgo_api_types-2023.7.5.6.44.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.06.08.15.39.07"
+version = "2023.07.05.06.44.07"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.6.8.15.39.7/PKG-INFO` & `fgo_api_types-2023.7.5.6.44.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.6.8.15.39.7
+Version: 2023.7.5.6.44.7
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

