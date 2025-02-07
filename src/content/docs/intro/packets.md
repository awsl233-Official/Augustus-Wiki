---
title: 数据包一览
---

## 接收包 (由服务端向客户端发送的数据包):
- **S00PacketKeepAlive**: 服务器向客户端发送的心跳包。用于确认客户端是否仍然在线。
- **S02PacketChat**: 用于服务器向客户端发送消息。
- **S03PacketTimeUpdate**: 用于同步服务端和客户端之间的游戏时间。
- **S04PacketEntityEquipment**: 用于更新实体的装备数据，比如玩家穿着的装备，物品栏中的武器/工具等。
- **S05PacketSpawnPosition**: 用于定义玩家的出生点位置。
- **S06PacketUpdateHealth**: 用于更新玩家的血量、饥饿值、饱和度数据。
- **S07PacketRespawn**: 用于强制玩家在死亡后/传送维度时重生。
- **S08PacketPlayerPosLook**: 用于更新玩家的位置/转头数据。
- **S09PacketHeldItemChange**: 用于更新玩家当前手持物品。
- **S0APacketUseBed**: 用于提醒客户端玩家使用了床。
- **S0BPacketAnimation**： 用于实体播放动画，如摆动手臂，受伤等。
- **S0CPacketSpawnPlayer**： 用于在世界中生成一个玩家实体。
- **S0DPacketCollectItem**： 用于提示客户端玩家捡起了物品。
- **S0EPacketSpawnObject**： 在世界中生成诸如箭矢，船只，鱼钩等物体。
- **S0FPacketSpawnMob**： 在世界上生成一个敌对实体。
- **S10PacketSpawnPainting**： 用于在世界中生成一个画实体。
- **S11PacketSpawnExperienceOrb**： 用于在世界中生成经验球。
- **S12PacketEntityVelocity**： 用于更新实体的速度。
- **S13PacketDestroyEntities**： 用于通知客户端从世界中移除一个实体。
- **S14PacketEntity**： 用于更新实体的位置和转头数据。
- **S15PacketEntityRelMove**： 用于提示客户端该实体相对于先前位置发生了移动。
- **S16PacketEntityLook**： 用于更新实体的头部旋转、身体旋转等数据。
- **S17PacketEntityLookMove**： 在S16的基础上，同时更新了位置数据。。
- **S18PacketEntityTeleport**： 用于将实体传送到特定位置。
- **S19PacketEntityHeadLook**： 仅更新实体的头部数据。
- **S1APacketEntityStatus**： 用于更新实体的状态，如着火或蹲下。
- **S1BPacketEntityAttach**： 用于实体的骑乘动作，如玩家驾驶矿车。
- **S1CPacketEntityMetadata**： 用于更新实体的NBT数据。
- **S1DPacketEntityEffect**： 用于对实体施加药水效果，如中毒或速度。
- **S1EPacketRemoveEntityEffect**: 用于移除实体的药水效果.
- **S20PacketEntityProperties**： 用于更新实体的属性，如健康、移动速度或攻击伤害。
- **S21PacketChunkData**： 用于向客户端发送区块数据。
- **S22PacketMultiBlockChange**： 用于修改一个区块内的多个方块。
- **S23PacketBlockChange**： 用于更新单个方块的状态。
- **S24PacketBlockAction**： 用于方块交互，如打开箱子或使用音符盒。
- **S25PacketBlockBreakAnim**： 用于显示破坏方块动画。
- **S26PacketMapChunkBulk**： 用于一次向客户端发送多个区块数据。
- **S27PacketExplosion**： 通过移除或破坏方块来模拟爆炸。
- **S28PacketEffect**： 发送爆炸或传送门声音等效果。
- **S29PacketSoundEffect**： 向客户端发送声音事件。
- **S2APacketParticles**： 发送粒子效果，如烟雾或火焰。
- **S2BPacketChangeGameState**： 改变游戏状态，如开始下雨或清除雨水。
- **S2CPacketSpawnGlobalEntity**： 生成一个全局实体，如闪电。
- **S2DPacketOpenWindow**： 打开一个窗口，如箱子或制作台界面。
- **S2EPacketCloseWindow**： 关闭客户端打开的窗口或图形用户界面。
- **S2FPacketSetSlot**： 更新特定库存槽中的物品。
- **S30PacketWindowItems**： 发送打开窗口库存中的所有物品。
- **S31PacketWindowProperty**： 更新窗口的属性，如酿造或熔炉图形用户界面中的进度条。
- **S32PacketConfirmTransaction**: 用于确认一次数据包传输的进行。
- **S33PacketUpdateSign**: 用于更新告示牌上的文字。
- **S34PacketMaps**: 用于向客户端发送地图数据。
- **S35PacketUpdateTileEntity**: 用于更新方块实体的数据，如箱子或熔炉。
- **S36PacketSignEditorOpen**: 用于打开客户端的告示牌编辑界面。
- **S37PacketStatistics**: 用于向客户端发送统计数据。
- **S38PacketPlayerListItem**: 用于更新tab栏中的玩家。
- **S39PacketPlayerAbilities**: 用于更新玩家的状态属性，如是否可以飞行，是否处于创造模式等。
- **S3APacketTabComplete**: 用于向客户端更新tab补全的数据。
- **S3BPacketScoreboardObjective**: 用于更新计分栏的内容。
- **S3CPacketUpdateScore**: 用于更新计分板各项内容的分数。
- **S3DPacketDisplayScoreboard**: 用于控制计分板是否显示。
- **S3EPacketTeams**： 用于管理计分板的队伍数据。
- **S3FPacketCustomPayload**： 用于向客户端发送自定义的数据信息。
- **S40PacketDisconnect**： 用于强制断开玩家的连接。
- **S41PacketServerDifficulty**： 用于更新服务器的难度。
- **S42PacketCombatEvent**： 用于控制战斗事件，如进入或离开战斗。
- **S43PacketCamera**： 用于改变玩家的摄像机视角，如作为观察者附身别人。
- **S44PacketWorldBorder**： 用于更新世界边界设置。
- **S45PacketTitle**： 用于在屏幕上显示标题。
- **S46PacketSetCompressionLevel**： 用于设置数据包的压缩阈值。
- **S47PacketPlayerListHeaderFooter**： 用于更新玩家列表的页眉和页脚内容。
- **S48PacketResourcePackSend**： 用于向客户端发送资源包 URL 供客户端下载。
- **S49PacketUpdateEntityNBT**： 用于发送实体的更新 NBT 数据。

## 发送包 (由客户端向服务端发送的数据包):
- **C00PacketKeepAlive**： 客户端向服务器发送的心跳包，用于确认客户端仍然在线。
- **C01PacketChatMessage**： 用于从客户端向服务器发送聊天信息。
- **C02PacketUseEntity**： 用于与实体交互，如攻击实体或与实体交互。
- **C03PacketPlayer**：基础的玩家数据包。
- **C04PacketPlayerPosition**： 用于向服务器发送玩家的位置数据。
- **C05PacketPlayerLook**： 用于发送玩家的转头数据（yaw & pitch）。
- **C06PacketPlayerPosLook**： 同时发送位置和转头数据。
- **C07PacketPlayerDigging**： 当玩家开始或完成挖掘方块时发送。
- **C08PacketPlayerBlockPlacement**： 当玩家在世界中放置方块时发送。
- **C09PacketHeldItemChange**： 向服务器通知修改了手中物品。
- **C0APacketAnimation**： 向服务器通知播放了动画。
- **C0BPacketEntityAction**： 发送实体动作，如蹲下或疾跑。
- **C0CPacketClickWindow**： 用于点击物品栏。当点击物品栏中的物品时发送。
- **C0DPacketCloseWindow**： 关闭物品栏。
- **C0EPacketClickWindow**： 确认物品栏的物品被点击。
- **C11PacketEnchantItem**： 物品附魔时发送。
- **C12PacketUpdateSign**： 更新告示牌文本。
- **C13PacketPlayerAbilities**： 发送玩家状态数据，如允许飞行或开启创造模式。
- **C14PacketTabComplete**： 请求服务器提供Tab补全数据。
- **C15PacketClientSettings**： 发送玩家的客户端设置，如语言、聊天可见性和渲染距离。
- **C16PacketClientStatus**： 更新客户端状态，如请求统计数据或复活。
- **C17PacketCustomPayload**： 发送自定义数据信息。
- **C18PacketSpectate**： 当玩家开始观战另一个实体时发送。
- **C19PacketResourcePackStatus**： 当玩家接受或拒绝资源包时发送。
- **CAnimateHandPacket**： 模拟高版本玩家的挥手动画。

这些数据包代表了 Minecraft 中客户端和服务器之间交换的各种操作和数据，包括移动、战斗、世界交互和游戏状态等。

## EntityActionsToCancel:
These are actions associated with an entity's behavior, particularly the player, and they likely correspond to player actions that can be canceled.

- **StartSprint**: Indicates that the player begins sprinting.
- **StopSprint**: Indicates that the player stops sprinting.
- **StartSneaking**: Signals that the player begins sneaking (crouching).
- **StopSneaking**: Signals that the player stops sneaking.
- **StopSleeping**: Indicates that the player has stopped sleeping, likely when exiting a bed.
- **RidingJump**: Used when the player performs a jump while riding an entity (e.g., a horse or pig).
- **OpenInventory**: Triggers when the player opens their inventory.

## DiggingPacket:
These are related to the block digging or destruction process, typically handled when the player interacts with blocks.

- **StartDestroyBlock**: Indicates the player has started breaking a block.
- **AbortDestroyBlock**: Cancels the block destruction process, such as when the player stops mining mid-way.
- **StopDestroyBlock**: Sent when the block is fully destroyed by the player.
- **DropAllItems**: Causes the player to drop all items from their inventory.
- **DropItem**: Drops a single item from the player’s inventory.
- **ReleaseUseItem**: Indicates that the player has stopped using an item (e.g., releasing a bowstring after drawing the bow).

These packets are key to handling player actions related to movement, block breaking, and interactions with their inventory or items.
