## Dell Inspiron 7590/7591 Hackintosh Guidance

 [![Group Badge](https://img.shields.io/badge/Chat%20on-Telegram-419fd9)](https://t.me/hackintosh759x) [![https://img.shields.io/badge/English%20version-here-blue](https://img.shields.io/badge/English%20version-here-blue)](https://github.com/Skimige/Inspiron-759x-Hackintosh/blob/master/README_en.md)

### 分享的 EFI

我们最推荐的是 saintno1997 (GitHub @tctien342) 维护的 EFI。虽然是 7591，但实测 7590 也可以使用。

Pinming 的版本是从 saintno 的版本修改而来。

| 分享者      | 对应机种 | 下载链接                                                     |
| ----------- | -------- | ------------------------------------------------------------ |
| saintno1997 | 7591     | [GitHub](https://github.com/tctien342/Dell-Inspiron-7591-Hackintosh) |
| Pinming     | 7590 4K  | [GitHub](https://github.com/Pinming/Dell-Inspiron-7590-Hackintosh-Opencore) |

鉴于部分 EFI 没有得到较好的维护且已经比较旧，并且已经有了频繁更新的版本，故将其折叠在下方。

<details>
    <summary>过时 EFI</summary>
<table>
<thead>
<tr>
<th>分享者</th>
<th>对应机种</th>
<th>下载链接</th>
</tr>
</thead>
<tbody>
<tr>
<td>Skimige</td>
<td>7590 4K</td>
<td><a href="https://caomsacid0-my.sharepoint.com/:u:/g/personal/skimige_caoms_ac_id/EePW1NdVOPpOpwrPUUMvwhIBDjzTnVIh7RNxnEGvvUbUeQ?e=qJGOA5" rel="nofollow">OneDrive</a></td>
</tr>
<tr>
<td>LinZong</td>
<td>7590 1080p</td>
<td><a href="https://github.com/LinZong/dell-inspiron-7590-hackintosh">GitHub</a></td>
</tr>
<tr>
<td>chtzs</td>
<td>7590 4K</td>
<td><a href="https://gitee.com/chtzs/Dell-Inspiron-7590-4k-Hackintosh" rel="nofollow">Gitee</a></td>
</tr>
<tr>
<td>kawauso</td>
<td>7590 4K</td>
<td><a href="https://github.com/sotyou/Dell-Inspiron-7590-Mojave">GitHub</a></td>
</tr>
<tr>
<td>missile0407</td>
<td>7590 1080p</td>
<td><a href="https://www.tonymacx86.com/threads/nearly-success-catalina-on-dell-inspiron-7590.285606/" rel="nofollow">tonymacx86</a></td>
</tr>
</tbody>
</table>
</details>
### 也许有用的文章 or 帖子

- [Dell Inspiron 7590 顶配版不负责评测 - Skimige's Blog](https://ikevin.in/post/2019/08/06/005-dell-inspiron-7590-4k-review.html)
- [DW1820A/BCM94350ZAE/BCM94356ZEPA50DX 插入的正确姿势 - 黑果小兵的部落阁]( https://blog.daliansky.net/DW1820A_BCM94350ZAE-driver-inserts-the-correct-posture.html)
- [XPS 15 杀手？ - Dell Inspiron 7591 体验报告 - tsuBench](https://telegra.ph/Dell-Inspiron-7591-07-08)
- [卡 `apfs_module_start` 的解决方法 - PCBeta](http://bbs.pcbeta.com/viewthread-1809664-1-1.html)
- [也许是首发，凑合用的 Dell Inspiron 7590 4k 配置的 Clover - PCBeta (By chtzs)](http://bbs.pcbeta.com/viewthread-1824495-1-1.html)
- 上面的 tonymacx86 帖子（折叠在「过时 EFI」中）和 [这个帖子](https://www.tonymacx86.com/threads/dell-inspiron-7590-hdmi-output-no-signal.284317/post-2013569)

### 特性

| 支持 | 名称          | 备注                                                         |
| ---- | ------------- | ------------------------------------------------------------ |
| 部分 | 声卡          | 内置麦克风未驱动（线路输入和 Type-C 可正常使用）；<br />ComboJack 需要修复，参考 saint 的 [ComboJack](https://github.com/tctien342/Dell-Inspiron-7591-Hackintosh/tree/master/ComboJack%20Alc295) |
| 替换 | 网卡          | DW1820A 建议的型号是 `CN-0VW3T3 BCM94350ZAE ~:0021`；不可使用 DW1830（超宽）；<br />如果手头宽裕建议考虑更加稳定的 DW1560（~RMB 300+） |
| 否   | 指纹识别      | 一辈子都不可能支持的.jpg                                     |
| 是   | 亮度调节      | 经映射修复后可以使用原按键（Fn + F6/F7）调节                 |
| 部分 | 睡眠          | 可能会睡死，取决于 config 等                                 |
| 是   | 触控板        | 轮询和 GPIO 中断均可用                                       |
| 是   | Thunderbolt 3 | 显卡坞 + 5700XT 群友测试可识别（感谢 @missile0407），应该没什么问题 |
| 部分 | HDMI          | 音频输出有问题等；如果配置得好，可能会解决大部分问题         |
| …    | …             | …                                                            |
