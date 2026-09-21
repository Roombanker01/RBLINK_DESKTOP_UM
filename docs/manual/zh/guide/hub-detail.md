# Hub 详情

## 防护与日志

**Disarm**、**Arm Stay**、**Arm Away** 彼此互斥。确认目标 Hub 后选择一个标准状态，并以刷新后的状态为准。自定义防区独立于标准状态，最多 8 个，按后台定义名称显示，每个均可独立启用或取消。这是安全敏感操作，离开前请再次核对 Hub 和刷新后的状态。

已有 10 条日志时，**Get Log** 会被阻止并提示先删除旧日志。可用日志的 **Download** 会直接开始下载。请求或删除后请以刷新后的列表确认结果。

![Hub 标准防护确认：1 后果](/images/hubs/hub-standard-arm-confirm.png){.manual-shot}

| 编号 | 控件 | 结果或风险 |
|---|---|---|
| 1 | 确认信息 | 核对选定的标准模式和目标 Hub。 |
| 2 | 取消 | 关闭且不改变防护。 |
| 3 | 确认 | 发送选定的标准防护变更。 |

![Hub 自定义防区确认：1 后果](/images/hubs/hub-custom-defence-confirm.png){.manual-shot}

| 编号 | 控件 | 结果或风险 |
|---|---|---|
| 1 | 确认信息 | 核对命名自定义防区和目标 Hub。 |
| 2 | 取消 | 关闭且不改变自定义防区。 |
| 3 | 确认 | 发送选定的自定义防区变更。 |

![Hub 日志上限提示：1 提示](/images/hubs/hub-log-limit-warning.png){.manual-shot}

| 编号 | 控件 | 结果 |
|---|---|---|
| 1 | Get Log | 达到 10 条上限时请求不会创建新日志。 |
| 2 | 警告信息 | 请先删除旧日志再请求新日志。 |

![Hub 详情：1 Hub 列表，2 Hub 详情，3 Remote Config，4 子设备，5 添加子设备，6 编辑，7 Disarm，8 Arm Stay，9 Arm Away，10 Perimeter，11 Night Watch](/images/hubs/hub-detail-main.png){.manual-shot}

| 编号 | 控件 | 前置、操作、结果、失败或权限 |
|---|---|---|
| 1 | Hub 列表 | 返回 Hub 列表。 |
| 2 | Hub 详情 | 显示选定 Hub 的名称、SN、归属、状态和当前可用控件。 |
| 3 | Remote Config | 打开选定 Hub 的配置。用户、SSH 和重启控件受角色限制，另见对应章节。 |
| 4 | 子设备 | 打开选定 Hub 的子设备列表；不会物理删除任何设备。 |
| 5 | 添加子设备 | 打开子设备注册。 |
| 6 | 编辑 | 授权用户修改 Hub 名称或公司归属。请求被拒绝时原归属不变。 |
| 7 | Disarm | 打开该 Hub 的撤防确认；提交前核对目标和当前安防上下文。 |
| 8 | Arm Stay | 打开该 Hub 的 Arm Stay 确认。 |
| 9 | Arm Away | 打开该 Hub 的 Arm Away 确认。 |
| 10 | Perimeter | 已配置且启用时选择 Perimeter 自定义防区。 |
| 11 | Night Watch | 已配置且启用时选择 Night Watch 自定义防区。 |

![Hub 日志：1 下载，2 删除，3 获取日志，4 导出消息到 Excel，5 返回列表](/images/hubs/hub-detail-logs.png){.manual-shot}

| 编号 | 日志或导出控件 | 前置、操作、结果、失败或权限 |
|---|---|---|
| 1 | 下载 | 下载选定的可用日志。缺少下载信息或授权失败时会报告错误，不改变 Hub 归属。 |
| 2 | 删除 | 为选定日志打开删除确认；确认前不会删除。 |
| 3 | Get Log（获取日志） | 从 Hub 收集日志，成功后刷新列表；失败时原列表不变。 |
| 4 | Export Messages to Excel（导出消息到 Excel） | Export 卡片为该 Hub 消息发送导出请求。失败不会改变 Hub 或日志记录。 |
| 5 | 返回列表 | 返回 Hub 列表。 |

![删除 Hub 日志确认：1 警告，2 取消，3 OK](/images/hubs/hub-log-delete-confirm.png){.manual-shot}

| 编号 | 确认控件 | 用途和风险 |
|---|---|---|
| 1 | 警告 | 继续前确认显示的日志就是目标日志。 |
| 2 | 取消 | 关闭对话框，不删除日志。 |
| 3 | OK | 授权请求成功后只删除选定日志；不会解除 Hub 绑定、物理删除 SN 或删除子设备。 |
