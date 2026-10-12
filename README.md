# scoop-bucket

A [Scoop](https://scoop.sh) bucket for [wslbak](https://github.com/Boring206/wslbak): scheduled,
verified backups of a WSL distro without stopping it, and one-line restore.

```
scoop bucket add boring206 https://github.com/Boring206/scoop-bucket
scoop install wslbak
```

Later, `scoop update wslbak` brings a newer version.

`bucket/wslbak.json` is not edited by hand. Every wslbak release contains the manifest, written by
the workflow that built the zips; the workflow in this repository copies it here within a day of a
release, and then installs wslbak from the bucket on a Windows runner to check that it works.

---

[wslbak](https://github.com/Boring206/wslbak/blob/main/README-zh-TW.md) 的 [Scoop](https://scoop.sh) bucket。
wslbak 替 WSL distro 做排程備份：不用停機、每次備份完自動試還原，還原只要一行指令。

```
scoop bucket add boring206 https://github.com/Boring206/scoop-bucket
scoop install wslbak
```

之後用 `scoop update wslbak` 更新。

`bucket/wslbak.json` 不是手動編輯的。wslbak 每次發佈都附有這份清單，由建置 zip 的那個工作流程寫出；
這個 repo 的工作流程會在發佈後一天內把它複製過來，並在 Windows 的執行環境上實際從這個 bucket 安裝一次來確認。
