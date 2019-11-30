## Dell Inspiron 7590/7591 Hackintosh Guidance

 [![Group Badge](https://img.shields.io/badge/Chat%20on-Telegram-419fd9)](https://t.me/hackintosh759x) [![https://img.shields.io/badge/English%20version-here-blue](https://img.shields.io/badge/English%20version-here-blue)](https://github.com/Skimige/Inspiron-759x-Hackintosh/blob/master/README_en.md)

### 分享的 EFI

| 分享者      | 对应机种                                                     | 下载链接                                                     |
| ----------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Skimige     | 7590 4K                                                      | [OneDrive](https://caomsacid0-my.sharepoint.com/:u:/g/personal/skimige_caoms_ac_id/EePW1NdVOPpOpwrPUUMvwhIBDjzTnVIh7RNxnEGvvUbUeQ?e=qJGOA5) |
| LinZong     | 7590 1080p                                                   | [GitHub](https://github.com/LinZong/dell-inspiron-7590-hackintosh) |
| chtzs       | 7590 4K                                                      | [Gitee](https://gitee.com/chtzs/Dell-Inspiron-7590-4k-Hackintosh) |
| kawauso     | 7590 4K                                                      | [GitHub](https://github.com/sotyou/Dell-Inspiron-7590-Mojave) |
| saintno1997 | 7591 | [GitHub](https://github.com/tctien342/Dell-Inspiron-7591-Hackintosh)                                                             |
| missile0407 | 7590 1080p                                                   | [tonymacx86](https://www.tonymacx86.com/threads/nearly-success-catalina-on-dell-inspiron-7590.285606/) |

### 也许有用的文章 or 帖子

- [Dell Inspiron 7590 顶配版不负责评测 - Skimige's Blog](https://ikevin.in/post/2019/08/06/005-dell-inspiron-7590-4k-review.html)
- [DW1820A/BCM94350ZAE/BCM94356ZEPA50DX 插入的正确姿势 - 黑果小兵的部落阁]( https://blog.daliansky.net/DW1820A_BCM94350ZAE-driver-inserts-the-correct-posture.html)
- [XPS 15 杀手？ - Dell Inspiron 7591 体验报告 - tsuBench](https://telegra.ph/Dell-Inspiron-7591-07-08)
- [卡 `apfs_module_start` 的解决方法 - PCBeta](http://bbs.pcbeta.com/viewthread-1809664-1-1.html)
- [也许是首发，凑合用的 Dell Inspiron 7590 4k 配置的 Clover - PCBeta (By chtzs)](http://bbs.pcbeta.com/viewthread-1824495-1-1.html)
- 上面的 tonymacx86 帖子和 [这个帖子](https://www.tonymacx86.com/threads/dell-inspiron-7590-hdmi-output-no-signal.284317/post-2013569)

### 特性

| 支持 | 名称          | 备注                                                         |
| ---- | ------------- | ------------------------------------------------------------ |
| 部分 | 声卡          | 麦克风未驱动；ComboJack 可能需要修复                         |
| 替换 | 网卡          | DW1820A 建议 `CN-0VW3T3 BCM94350ZAE ~:0021`；不可使用 DW1830（超宽） |
| 否   | 指纹识别      | 一辈子都不可能支持的.jpg                                     |
| 是   | 亮度调节      | 经映射修复后可以使用原按键（Fn + F6/F7）调节                 |
| 部分 | 睡眠          | 可能会睡死                                                   |
| 是   | 触控板        | 轮询和 GPIO 中断均可用                                       |
| 是   | Thunderbolt 3 | 显卡坞 + 5700XT 群友测试可识别（感谢 @missile0407），应该没什么问题 |
| 部分 | HDMI          | 音频输出有问题等                                             |
| …    | …             | …                                                            |
