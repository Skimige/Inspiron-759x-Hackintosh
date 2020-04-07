## Dell Inspiron 7590/7591 Hackintosh Guidance

 [![Group Badge](https://img.shields.io/badge/Chat%20on-Telegram-419fd9)](https://t.me/hackintosh759x)

### Shared EFIs Collection

We recommend saintno's EFI most. Although its target model is 7591, 7590 can run perfectly under this EFI.

Pinming's EFI is a fork from saintno's with some edits.

| User        | Spec       | Download                                                     |
| ----------- | ---------- | ------------------------------------------------------------ |
| saintno1997 | 7591     | [GitHub](https://github.com/tctien342/Dell-Inspiron-7591-Hackintosh) |
| Pinming     | 7590 4K  | [GitHub (README in Chinese)](https://github.com/Pinming/Dell-Inspiron-7590-Hackintosh-Opencore) |

As some of the EFIs are no longer updated, and we've got these frequently updated EFI above, these EFIs are folded below.

<details>
    <summary>Outdated EFI</summary>
<table>
<thead>
<tr>
<th>User</th>
<th>Spec</th>
<th>Download</th>
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

### Posts that might be useful

*Notice: Most posts here are written in Chinese. Use a translator to help you.*

- [Dell Inspiron 7590 4K Review - Skimige's Blog](https://ikevin.in/post/2019/08/06/005-dell-inspiron-7590-4k-review.html)
- [DW1820A/BCM94350ZAE/BCM94356ZEPA50DX Correct Way to Enable - daliansky's Blog]( https://blog.daliansky.net/DW1820A_BCM94350ZAE-driver-inserts-the-correct-posture.html)
- [XPS 15 Killer? - Dell Inspiron 7591 Experience Report - tsuBench](https://telegra.ph/Dell-Inspiron-7591-07-08)
- [How to Solve stucking at `apfs_module_start` - PCBeta](http://bbs.pcbeta.com/viewthread-1809664-1-1.html)
- [A Clover for Dell Inspiron 7590 4k - PCBeta (By chtzs)](http://bbs.pcbeta.com/viewthread-1824495-1-1.html)
- the tonymacx86 posts above (In "Outdated EFI" Section) and [this one](https://www.tonymacx86.com/threads/dell-inspiron-7590-hdmi-output-no-signal.284317/post-2013569)

### Features

| Status  | Name          | Note                                                         |
| ------- | ------------- | ------------------------------------------------------------ |
| Partial | Audio         | Internal Mic is not working (Line-in and Type-C are working properly);<br />ComboJack need fixup, please refer to saint's [ComboJack](https://github.com/tctien342/Dell-Inspiron-7591-Hackintosh/tree/master/ComboJack%20Alc295) |
| Replace | NIC           | Suggested DW1820A model is: `CN-0VW3T3 BCM94350ZAE ~:0021`;<br />don't use DW1830, its width is wider than the free space;<br />if you get enough money, use DW1560 which is much more stable and easy to configurate (~USD 60) |
| No      | Fingerprint   | Impossible to add support, lol                               |
| Yes     | Brightness    | Can use Fn + F6/F7 to change after SSDT mapping fixup        |
| Partial | Sleep         | May reboot when waking, depending on your config             |
| Yes     | Touchpad      | Polling or GPIO, both OK.                                    |
| Yes     | Thunderbolt 3 | Should work. Tested AMD 5700XT and can be identified by macOS (credit @missile0407). |
| Partial | HDMI          | Audio output problems; If well configured could work better  |
| …       | …             | …                                                            |

