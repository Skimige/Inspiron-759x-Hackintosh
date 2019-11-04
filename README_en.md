## Dell Inspiron 7590/7591 Hackintosh Guidance

 [![Group Badge](https://img.shields.io/badge/Chat%20on-Telegram-419fd9)](https://t.me/hackintosh759x)

### Shared EFIs Collection

| User        | Spec       | Download                                                     |
| ----------- | ---------- | ------------------------------------------------------------ |
| Skimige     | 7590 4K    | [OneDrive](https://caomsacid0-my.sharepoint.com/:u:/g/personal/skimige_caoms_ac_id/EePW1NdVOPpOpwrPUUMvwhIBDjzTnVIh7RNxnEGvvUbUeQ?e=qJGOA5) |
| LinZong     | 7590 1080p | [GitHub](https://github.com/LinZong/dell-inspiron-7590-hackintosh) |
| chtzs       | 7590 4K    | [Gitee](https://gitee.com/chtzs/Dell-Inspiron-7590-4k-Hackintosh) |
| kawauso     | 7590 4K    | [GitHub](https://github.com/sotyou/Dell-Inspiron-7590-Mojave) |
| saintno1997 | 7591       | [GitHub](https://github.com/tctien342/Dell-Inspiron-7591-Hackintosh) |
| missile0407 | 7590 1080p | [tonymacx86](https://www.tonymacx86.com/threads/nearly-success-catalina-on-dell-inspiron-7590.285606/) |

### Posts that might be useful

Notice: Most posts here are written in Chinese. Use a translator to help you.

- [Dell Inspiron 7590 4K Review - Skimige's Blog](https://ikevin.in/post/2019/08/06/005-dell-inspiron-7590-4k-review.html)
- [DW1820A/BCM94350ZAE/BCM94356ZEPA50DX Correct Way to Enable - daliansky's Blog]( https://blog.daliansky.net/DW1820A_BCM94350ZAE-driver-inserts-the-correct-posture.html)
- [XPS 15 Killer? - Dell Inspiron 7591 Experience Report - tsuBench](https://telegra.ph/Dell-Inspiron-7591-07-08)
- [How to Solve stucking at `apfs_module_start` - PCBeta](http://bbs.pcbeta.com/viewthread-1809664-1-1.html)
- [A Clover for Dell Inspiron 7590 4k - PCBeta (By chtzs)](http://bbs.pcbeta.com/viewthread-1824495-1-1.html)
- the tonymacx86 posts above and [this one](https://www.tonymacx86.com/threads/dell-inspiron-7590-hdmi-output-no-signal.284317/post-2013569)

### Features

| Status  | Name          | Note                                                         |
| ------- | ------------- | ------------------------------------------------------------ |
| Partial | Audio         | Mic is not working; ComboJack may need fixup                 |
| Replace | NIC           | Suggested DW1820A: `CN-0VW3T3 BCM94350ZAE ~:0021`; don't use DW1830, its width is wider than the free space |
| No      | Fingerprint   | Impossible to add support lol                                |
| Yes     | Brightness    | Can use Fn + F6/F7 to change after SSDT mapping fixup        |
| Partial | Sleep         | May reboot when waking                                       |
| Yes     | Touchpad      | Polling or GPIO, both OK.                                    |
| Yes(?)  | Thunderbolt 3 | Waiting for more tests. Tested AMD 5700XT and can be identified by macOS (credit @missile0407); USB 3 fully working |
| Partial | HDMI          | Audio output problems                                        |
| …       | …             | …                                                            |

