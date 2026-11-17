# Faren NPC 汉化说明

## 模组信息

| 项目 | 内容 |
| --- | --- |
| 模组名称 | Faren（法伦·布莱克诺，BG2 可恋爱 NPC） |
| 模组根目录 | `E:\GitHub\Faren-NPC\faren` |
| 主安装文件 | `setup-faren.tp2`（AUTHOR 指向 spellholdstudios，`VERSION @132`） |
| 适用游戏 | Baldur's Gate II（SoA + ToB，含 EET） |
| 原作语言 | 英文（`translations\english`，42 个 .TRA） |

## 汉化范围

- 仅翻译**译文层**：`translations\english` 的 42 个 .TRA 全部译入 `translations\schinese`。
- 英文原文（`translations\english`）**未作任何修改**，保留作为回退与对照。
- `setup-faren.tp2` **本次汉化未改动**。（工作区中该文件已存在 `LANGUAGE ~Schinese~ ~schinese~ ~Faren/translations/schinese/setup.tra~` 条目，属本仓库既有改动，非本次汉化产生；汉化文件即按该条目所指路径存放。）
- 未新增 `.bak` 备份；`audio`、`graphics`、`items`、`creatures`、`lib`、`script`、`dialogues` 等资源与代码目录未触碰。
- 涵盖范围：主线对话（`fhfrn` / `bfhfrn` / `bfhf25`）、SoA 关系与闲聊大文件（`fhfrnj`）、ToB 版关系文件（`fhf25j` / `fhf25`）、反应与随机对话（`fhfreact` / `fhfq` / `fhflux`）、日记（`journals`）、安装界面与物品说明（`setup`），以及 30 余个 **crossmod** 队友互动文件（Amber、Ajantis、Angelo、Aurenaseph、Chloe、Edwin、Fade、Iylos、Kelsey、Keto、Luxley、Nalia、Nathaniel、Ninde、Saerileth、Sarah、Solaufein、Seth、Tsujatha、Xan、Xulaye、Yasraena 等）。

## 编码与换行

- 输出编码：**UTF-8（无 BOM）**，换行 **CRLF**。
- 依据：`setup-faren.tp2` 使用 `AUTO_TRA ~Faren/translations/%s~` 直读译文，模组内**没有任何 `HANDLE_CHARSETS` / iconv 转码层**，因此 UTF-8 中文可直接被 WeiDU 读取，无需转码；反之若存 ANSI(GBK) 会触发 `LEXER ERROR: invalid character`。
- 全部 42 个文件已逐字节校验：均无 BOM，且换行全部为 CRLF（无孤立 LF）。

## 文件与条目统计

合计 **42 个 .TRA / 5403 条**，全部完成。

| 文件 | 条目数 |
| --- | --- |
| fhfrnj.tra | 2454 |
| fhf25j.tra | 821 |
| bfhfrn.tra | 439 |
| bfhf25.tra | 191 |
| fhfreact.tra | 160 |
| fhfrn.tra | 159 |
| setup.tra | 152 |
| fhfq.tra | 138 |
| fhflux.tra | 115 |
| fhfseth.tra | 79 |
| fhfnath.tra | 48 |
| fhfnind.tra | 47 |
| fhfklsy.tra | 44 |
| fhfsl.tra | 43 |
| fhfxan.tra | 41 |
| fhfang.tra | 39 |
| fhfaj.tra | 35 |
| fhfchloe.tra | 33 |
| fhfsol.tra | 32 |
| fhf25.tra | 31 |
| fhfketo.tra | 26 |
| fhfamb.tra | 25 |
| fhfrnp.tra | 25 |
| fhfsr.tra | 24 |
| fhffade.tra | 21 |
| fhfnal.tra | 21 |
| fhfaur.tra | 19 |
| fhftsu.tra | 17 |
| fhfiylos.tra | 15 |
| fhfyas.tra | 14 |
| fhf25p.tra | 13 |
| fhfxul.tra | 11 |
| fhfang25.tra | 9 |
| fhfedwin.tra | 9 |
| fhfkls25.tra | 9 |
| fhfn25.tra | 8 |
| fhfx25.tra | 8 |
| fhfaur25.tra | 7 |
| fhfsl25.tra | 6 |
| fhfyas25.tra | 6 |
| fhfsr25.tra | 5 |
| journals.tra | 4 |

> 编号说明：`setup.tra`（编号 0–157 实际 152 条）、`fhfq.tra`（0–200 实际 138 条）、`fhf25j.tra`（缺 @429）、`fhfrnj.tra`（0–2454 实际 2454 条）等源文件本身存在跳号，译文**完全沿用源文件编号，未补号、未重排**。

## 术语表（关键译名，全书统一）

- 人物：Faren 法伦（Faren Blacknall 法伦·布莱克诺）｜Saerileth 莎丽蕾丝｜Kelsey 凯尔西（Coltrane 柯川）｜Solaufein 索劳芬｜Yasraena 雅丝琳娜｜Tsujatha 楚加莎｜Xan 赞｜Nathaniel 纳萨尼尔｜Amber 安柏｜Ajantis 阿詹提斯｜Angelo 安吉罗｜Auren/Aurenaseph 奥伦｜Chloe 克洛伊｜Edwin 艾德温｜Fade 法德｜Iylos 伊洛斯｜Keto 琪托｜Luxley 卢克斯利｜Ninde 宁德｜Sarah 莎拉｜Seth 赛斯｜Xulaye 舒拉耶｜Nalia 娜里亚｜Imoen 爱蒙｜Jaheira 贾希拉（Khalid 卡立德）｜Viconia 维康妮亚｜Aerie 爱黎｜Anomen 安诺门｜Mazzy 玛兹｜Valygar 瓦尔加｜Yoshimo 吉见｜Haer'Dalis（对白中自称“我的猎犬”）｜Jan Jansen 姚恩·詹森｜Bodhi 波迪｜Irenicus 爱瑞尼克斯｜Elhan 艾尔汉｜Gorion 葛立安｜Arkanis 阿卡尼斯
- 本模组独有 NPC：Jarvis 贾维斯（贸易集会卫队长）｜Cooper 库珀｜Isaac 艾萨克｜Jeanne 珍妮｜Vyatri 维亚特里（Vyatri's 维亚特里酒馆）｜Raissa 莱莎｜Halmar 哈尔玛｜Linnea Belka 琳妮娅·贝尔卡｜Menold 梅诺德｜Lord Coprith 科普里斯大人｜Lilpole 利尔波尔（剧作家，剧作《特里安娜》）｜Nadiyya 纳迪雅（猫）｜Felix 菲力克斯（雪貂）｜Wallace 华莱士｜Madame Nin 宁夫人｜Lilith 莉莉丝夫人｜Xavier 泽维尔｜Andrei 安德烈｜Sebastian 塞巴斯蒂安｜Jessalyn 杰莎琳（昵称 Jessa 杰莎）
- 地名/机构：Athkatla 阿斯卡特拉｜Trademeet 贸易集会｜Imnesvale 伊姆斯维尔｜Umar Hills 乌玛丘陵｜Underdark 幽暗地域｜Ust Natha 乌斯特·纳萨｜Saradush 萨拉杜什｜Amn 安姆｜Tethyr 泰西尔｜Chult 楚尔特｜Luskan 卢斯坎｜Baldur's Gate 博德之门｜Candlekeep 烛堡｜Copper Coronet 铜冠酒馆｜Waukeen's Promenade 沃金步道｜Temple of Waukeen 沃金神庙（Waukeen 沃金）｜Graveyard District 墓地街区｜Docks 码头区｜Shadow Thieves 影贼｜Cowled Wizards 斗篷法师｜Order of the Radiant Heart 光辉之心骑士团｜Rhynn Lanthorn 琳恩灯笼｜Slayer 杀戮者｜Bhaalspawn 巴尔之子｜Oghma 奥格玛（Binder of What is Known 已知之束缚者）
- 其他：almond brandy 杏仁白兰地｜Black Lotus 黑莲花（兰花酒廊）｜rivvil 里夫维尔（卓尔语“地表人”）｜pocket plane 口袋位面

## 保留不译

`<CHARNAME>`、`<PRO_RACE>`、`<PRO_HESHE>`、`<PRO_HIMHER>`、`<PRO_HISHER>`、`<PRO_BROTHERSISTER>`、`<PRO_MANWOMAN>`、`<PRO_GIRLBOY>`、`<PRO_BOYGIRL>`、`<PRO_LADYLORD>`、`<PRO_SIRMAAM>`、`<SIRMAAM>`、`<MALEFEMALE>`、`<DAYNIGHT>`、`<DAYNIGHTALL>` 等 WeiDU 变量标记全部原样保留在译文中，仅翻译其周边文字（如 “to<DAYNIGHT>” 译为 “<DAYNIGHT>” 前置的对应表达，标记本身不动），以便引擎按性别/昼夜正确替换。

## 校验记录

对 42 个文件逐条与英文源做独立比对（脚本 `verify.py` / `fixcheck.py` / `residue.py`），结果：

1. **条目编号集合**：42/42 与源文件完全一致（含源文件跳号情况）。
2. **波浪号数量**：42/42 为 `2 × 条目数`，无内部 `~`，无吞并下一行的情况（`fhfrnj.tra` 恒为 4908/4908）。
3. **物理行数**：42/42 与源一致，含多行条目（`fhfrnj` 2515 行、`fhf25j` 869 行、`fhfq` 157 行、`fhfreact` 166 行、`setup` 170 行、`journals` 21 行、`fhfseth` 87 行、`fhfrnp` 31 行），段落数与原文一一对应。
4. **占位符**：逐条比对 `<...>` 标记集合，42/42 完全一致（曾发现 44 处漏掉 `<DAYNIGHT>` / `<PRO_HISHER>` / `<DAYNIGHTALL>` / `<PRO_MANWOMAN>` 的条目，已全部回补并复验通过）。
5. **编码/换行**：42/42 无 BOM，纯 CRLF，无孤立 LF。
6. **英文残留**：逐条检查“源含英文单词但译文无汉字”的条目，结果为 0（3 条漏译已补齐）。
7. **译文瑕疵修正**：`fhfrnj @1402` 漏字（“你还对想入非非”→“你还对她想入非非”）已改；`fhf25j`/`fhfrnj` 中字面量 `\n` 转义未落地的 166 处已统一转为真实换行。

## 备注

- 全文为中文玩家语境下的意译，保留法伦“痞气自嘲 + 底层出身”的口吻；粗口按原文强度对应（damn→该死、bastard→混蛋等），未作删弱也未加码。
- 同一段落中存在大量仅差一两词的**重复变体条目**（如 `fhfrnj` @137/@384、@9/@20/@21/@24 等），已逐条独立翻译并保留其细微语义差，未合并、未留空。
- `fhfrnj` 与 `fhf25j` 含大量 `(He grins...)` 式第一人称旁白与玩家短选项（`(Flirt with Faren.)`、`(Kiss Faren.)`、`(Wolf whistle at Faren.)` 等），旁白统一用全角括号，选项统一用“（动作。）”格式。
- 安装时选择 **Schinese** 语言即可；若游戏为中文版 EET，语言列表显示名称沿用模组自带 `LANGUAGE ~Schinese~`。
