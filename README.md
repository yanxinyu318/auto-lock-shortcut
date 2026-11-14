# 自动锁定切换

iPhone 快捷指令：在“切到永不 / 切到 2 分钟”之间切换自动锁定。

iOS 快捷指令里没有直接改自动锁定时间的动作，所以这个快捷指令的做法是：
运行后弹出菜单让用户选方向 → 弹窗提示该点哪个 → 打开“设置 → 显示与亮度 → 自动锁定”页（`prefs:root=DISPLAY&path=AUTOLOCK`），用户在设置里手动点一下。

## 签名

仓库里 `自动锁定切换.shortcut` 是未签名文件，iPhone 会拒绝导入。
去 Actions → Sign Shortcut → Run workflow，跑完后在 Artifacts 里下载 `signed-shortcut`，
里面就是签过名的 `自动锁定切换.shortcut`，在 iPhone 上点开即可导入。
