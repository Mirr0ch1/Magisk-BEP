# Extra GMS features for H2OS Android P

The `ContactsSyncAdapter` and `BackupTransport` are missing in the first release of OnePlus's H2OS 9.0(Android P) for OnePlus 5 in Mainland China. In result, contacts and backup data can not be retrieved after a clean installation.

## Containing

```
/system/app/GoogleExtShared/GoogleExtShared.apk
/system/etc/default-permissions/backuptransport-permissions.xml
/system/etc/permissions/com.google.android.maps.xml
/system/etc/permissions/com.google.android.media.effects.xml
/system/etc/permissions/privapp-permissions-backuptransport.xml
/system/etc/permissions/privapp-permissions-gsfext.xml
/system/etc/sysconfig/google_backuptransport.xml
/system/framework/com.google.android.maps.jar
/system/framework/com.google.android.media.effects.jar
/system/priv-app/ConfigUpdater/ConfigUpdater.apk
/system/priv-app/GoogleBackupTransport/GoogleBackupTransport.apk
/system/priv-app/GoogleContactsSyncAdapter/GoogleContactsSyncAdapter.apk
/system/priv-app/GoogleExtServices/GoogleExtServices.apk
/system/priv-app/GoogleRestore/GoogleRestore.apk
/system/reserve/GoogleCalendarSyncAdapter-CBP/GoogleCalendarSyncAdapter-CBP.apk
```

### Changelog

- v1.1.6: Remove `DigitalWellbeing` due to compatibility issue with H2OS
- v1.1.4: First stable release with refined readme file
- v1.1.2: All functions working fine (the lolipop version of ContactsSyncAdapter downloaded from apkmirror.com is adapted)
- v1.0.8: `DigitalWellbeing` added
- v1.0.4: BackupTransport working properly, while ContactsSyncAdapter not
- v1.0.1: Initial release, all functions failed

## Be advised

- **If there's still no contact syncing option under account setting, please install the `ContactsSyncAdapter-CBP.apk` manually from `/system/reserve/GoogleContactsSyncAdapter-CBP` using any file manager with root access**.
- I will do my personal effort urging OnePlus to make the proper implementation of those features mentioned above.
- OnePlus sucks.

---

# 适用于 Android P H2OS 的额外 Google 组件

一加手机5 终于收到了第一版官方 Android P（氢OS 9.0）的推送，然而在该版中缺失了 Google 的 `ContactsSyncAdpater` 与 `BackupTransport` ，导致联系人信息与备份的应用数据在手机重置后无法恢复。本模块将重新安装这两个组件，顺便加入流行的 `DigitalWellbeing`。

## 包含内容

```
/system/app/GoogleExtShared/GoogleExtShared.apk
/system/etc/default-permissions/backuptransport-permissions.xml
/system/etc/permissions/com.google.android.maps.xml
/system/etc/permissions/com.google.android.media.effects.xml
/system/etc/permissions/privapp-permissions-backuptransport.xml
/system/etc/permissions/privapp-permissions-gsfext.xml
/system/etc/sysconfig/google_backuptransport.xml
/system/framework/com.google.android.maps.jar
/system/framework/com.google.android.media.effects.jar
/system/priv-app/ConfigUpdater/ConfigUpdater.apk
/system/priv-app/GoogleBackupTransport/GoogleBackupTransport.apk
/system/priv-app/GoogleContactsSyncAdapter/GoogleContactsSyncAdapter.apk
/system/priv-app/GoogleExtServices/GoogleExtServices.apk
/system/priv-app/GoogleRestore/GoogleRestore.apk
/system/reserve/GoogleCalendarSyncAdapter-CBP/GoogleCalendarSyncAdapter-CBP.apk
```

### 更新内容

- v1.1.6: 因氢OS 兼容问题移除「数字健康」
- v1.1.4: 完善说明，正式发布
- v1.1.2: 所有功能工作正常（采用了 5.1.1 版的 `ContactsSyncAdapter` ）
- v1.0.8: 增加喜闻乐见的「数字健康」
- v1.0.4: 备份传输组件工作正常，联系人同步无法使用
- v1.0.1: 第一版，联系人同步与备份传输组件均不可用

## 注意

- **若重启后依旧无通讯录同步选项，请使用文件浏览工具手动进入 `ContactsSyncAdapter-CBP` 放置目录将 apk 文件安装为用户应用**。
- 本人会积极推进一加在氢OS 固件分支内整合 ContactsSyncAdapter 与 BackupTransport。
- 辣鸡一加。
