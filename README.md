# 龙之剑：觉醒 — Aria 替换「泠鸢」mod

把《龙之剑：觉醒》中可操作角色 **阿莉娅（Aria）** 的模型替换成 **泠鸢**（MMD 模型），
提供两种外观：**公式服 3.0（栗子发）** 与 **素体**。
v1.1 起，游戏内的 **头像 / 立绘 / 图标（7 张 UI 图）** 也换成了同款 2D 立绘。

> 本仓库只放说明；pak 文件在 **Releases** 里下载。

## 版本一览（v1.1）

| 文件 | 大小 | SHA256 | 内容 |
|---|---|---|---|
| `zzzzDS_LingyuanGS_v1.0_full_P.pak` | 83,274,698 B | `16E0EC28…` | 公式服·完整版（仅移除裙摆上三块低像素装饰面板 `裙-金属`） |
| `zzzzDS_LingyuanGS_v1.0_nopants_P.pak` | 82,445,978 B | `40B83E80…` | 公式服·去安全裤 |
| `zzzzDS_LingyuanGS_v1.0_noback_pants_P.pak` | 79,646,656 B | `3D09D714…` | 公式服·去后带、保留安全裤（外裙+绳结+裤） |
| `zzzzDS_LingyuanGS_v1.0_slim_P.pak` | 81,161,008 B | `65482DC6…` | 公式服·精简版（外裙+绳结+后带，去掉袖/裤/裙内/金属/腿饰） |
| `zzzzDS_LingyuanXS_v1.0_P.pak` | 84,898,716 B | `7C148F05…` | 素体版 |

> 文件名沿用 `v1.0`（方便覆盖安装），实际内容已是 v1.1（含 UI 立绘）。

## 安装

1. 打开游戏目录：`<Steam>\steamapps\common\DragonSword  Awakening\DS\Content\Paks\`
2. 如果没有 `~mods` 文件夹，**手动新建一个**（名字必须是 `~mods`）
3. 把**其中一个** pak 复制进 `~mods\`
4. 重启游戏

> ⚠️ 同一时间只能装一个版本（它们替换同一套资产）。
> 与其他替换 Aria 的 mod 冲突，请先移除其它替换包。

## v1.1 更新内容

- 游戏内 **7 张 UI 图**全部换成同款 2D 立绘：`Icon_Character_Aria`（列表头像）、`Icon_Item_Character_Aria`（仓库图标）、`Img_Character_Mini_Aria`（小立绘）、`Img_Character_Key_Aria` / `KeyHalf` / `MainKeyHalf`（大立绘）、`Img_Character_Signal_Aria`（剪影）

## 已知限制

- **手指不会弯曲**（手掌固定跟随手腕）——后续版本会做手指弯曲
- 没有布料/头发物理（游戏自带物理不会驱动替换网格）
- 公式服裙摆前方原有的三块装饰面板（`裙-金属`）已移除：它们的贴图在合并图集后分辨率过低，会显示成低像素花纹
- 素体版布料权重沿用模型原始权重；公式服版布料按"离身体距离"分段跟随身体/裙骨

## 兼容性

- 游戏：龙之剑：觉醒（UE 5.3，Steam）
- 替换对象：阿莉娅 `ch_aria_mesh_body`（183 骨，A-pose）
- 包内不含 Skeleton，运行时使用游戏原骨架

## 版权

- 角色模型与立绘版权归原作者（泠鸢公式服3.0 by 临时映画 等），仅供个人游戏使用，请勿转载或商用
- 本 mod 的制作脚本与说明由 xpjlhxhkh 整理