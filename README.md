# QAudio
Audio playing library arranged with queues and priorities.

# Intro
This project is intended to integrade in large configuration softwares as
a audio playing library, such as alarms.

Main idea of this library is queues and priorities. As 8 different priorty
levels were integraded by the library, each priorty have a queue. When highest 
prioritied queue is empty, it automatically gets to the next queue to play
recursively. When the whole queue is empty, it stand by. High priorty queue
inserts a new piece, play the high priorty audio first. While one piece is
in play, it is not interruptable by priorty loop. But mannual control were
abled to interrupt.

# 介绍
该项目旨在集成到大型组态软件中，如
音频播放库，例如警报。

这个库的主要结构是队列和优先级。 有 8 个不同的优先级的队列由库集成，
每个优先级都有一个队列。 最高优先级的队列为空时，递归地自动进入下一
个队列播放。 当整个队列为空时，程序会等待新的音频加入队列。 高优先级
队列插入一个新片段时，首先播放高优先级音频。 虽然低优先级队列正在播
放中，库不会被高等级队列加入新音频打断。 但是音频的播放可以手动中断。
