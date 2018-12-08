# 适用于 Android P 的 Google 联系人同步与备份传输组件

一加手机5 终于收到了第一版官方 Android P（氢OS 9.0）的推送，然而在该版中缺失了 Google 的 `ContactsSyncAdpater` 与 `BackupTransport` ，导致联系人信息与备份的应用数据在手机重置后无法恢复。本模块将重新安装这两个组件。

## 包含内容

```
/system/app/GoogleContactsSyncAdapter/GoogleContactsSyncAdapter.apk
/system/priv-app/GoogleBackupTransport/GoogleBackupTransport.apk
```

## 注意

- 若系统环境已存在上述两个组件，则本模块 **不会对** 系统产生任何更改（即非强制挂载与替换）
- 本人会积极推进一加在氢OS 固件分支内整合 ContactsSyncAdapter 与 BackupTransport
- 辣鸡一加

---

# Google's Contacts Sync and Backup Transport for Android

The `ContactsSyncAdapter` and `BackupTransport` are missing in the first release of OnePlus's H2OS 9.0(Android P) for OnePlus 5 in Mainland China. In result, contacts and backup data can not be retrieved after a clean installation. This module will bring back those two features.

## Containing

```
/system/app/GoogleContactsSyncAdapter/GoogleContactsSyncAdapter.apk
/system/priv-app/GoogleBackupTransport/GoogleBackupTransport.apk
```

## Be advised

- If those two file already exist in your `/system` partition, this module will leave your device untouched.
- I will do my personal effort urging OnePlus to make the proper implementation of those features mentioned above.
- OnePlus sucks.
