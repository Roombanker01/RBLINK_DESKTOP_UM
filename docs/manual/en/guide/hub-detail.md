# Hub details

## Protection and logs

**Disarm**, **Arm Stay**, and **Arm Away** are mutually exclusive. Confirm the target Hub, choose one standard state, and use the refreshed status as the outcome. Custom defence zones are separate: up to eight administrator-named zones can be enabled or disabled independently. These are security-sensitive changes; verify the Hub and refreshed state before leaving.

When ten logs already exist, **Get Log** is blocked and asks you to delete an older log first. **Download** starts directly for an available log. Confirm any request or deletion from the refreshed list.

![Standard Hub protection confirmation: 1 consequence](/images/hubs/hub-standard-arm-confirm.png){.manual-shot}

| No. | Control | Result or risk |
|---|---|---|
| 1 | Confirmation message | Verify the selected standard mode and target Hub. |
| 2 | Cancel | Closes without changing protection. |
| 3 | Confirm | Sends the selected standard protection change. |

![Custom Hub defence confirmation: 1 consequence](/images/hubs/hub-custom-defence-confirm.png){.manual-shot}

| No. | Control | Result or risk |
|---|---|---|
| 1 | Confirmation message | Verify the named custom zone and target Hub. |
| 2 | Cancel | Closes without changing custom defence. |
| 3 | Confirm | Sends the selected custom defence change. |

![Hub log limit warning: 1 warning](/images/hubs/hub-log-limit-warning.png){.manual-shot}

| No. | Control | Result |
|---|---|---|
| 1 | Get Log | Requesting at the ten-log limit does not create another log. |
| 2 | Warning message | Delete an older log before requesting another. |

![Hub details: 1 Hub List, 2 Hub Detail, 3 Remote Config, 4 Sub-devices, 5 Add Sub-device, 6 Edit, 7 Disarm, 8 Arm Stay, 9 Arm Away, 10 Perimeter, 11 Night Watch](/images/hubs/hub-detail-main.png){.manual-shot}

| No. | Control | Prerequisite, action, result, failure or permission |
|---|---|---|
| 1 | Hub List | Returns to the Hub list. |
| 2 | Hub Detail | Shows the selected Hub's name, SN, ownership, status, and current controls. |
| 3 | Remote Config | Opens configuration for the selected Hub. Its user, SSH, and restart controls are role-gated and documented separately. |
| 4 | Sub-devices | Opens the selected Hub's sub-device list; it does not physically remove any device. |
| 5 | Add Sub-device | Opens registration for a sub-device. |
| 6 | Edit | Authorized users change the Hub name or company assignment. A rejected request leaves the prior assignment unchanged. |
| 7 | Disarm | Opens the disarm confirmation for the selected Hub. Confirm the target and current security context before submitting. |
| 8 | Arm Stay | Opens the Arm Stay confirmation for the selected Hub. |
| 9 | Arm Away | Opens the Arm Away confirmation for the selected Hub. |
| 10 | Perimeter | Selects the configured Perimeter custom defence when enabled. |
| 11 | Night Watch | Selects the configured Night Watch custom defence when enabled. |

![Hub logs: 1 Download, 2 Delete, 3 Get Log, 4 Export Messages to Excel, 5 Back to List](/images/hubs/hub-detail-logs.png){.manual-shot}

| No. | Log or export control | Prerequisite, action, result, failure or permission |
|---|---|---|
| 1 | Download | Downloads an available selected log. Missing download metadata or authorization failure reports an error without changing Hub ownership. |
| 2 | Delete | Opens the deletion confirmation for the selected log; it does not delete until confirmed. |
| 3 | Get Log | Collects logs from the Hub and refreshes the list after success. On failure, the current list remains unchanged. |
| 4 | Export Messages to Excel | The Export card sends an export request for this Hub's messages. Failure leaves the Hub and log records unchanged. |
| 5 | Back to List | Returns to the Hub list. |

![Delete Hub log confirmation: 1 warning, 2 Cancel, 3 OK](/images/hubs/hub-log-delete-confirm.png){.manual-shot}

| No. | Confirmation control | Use and risk |
|---|---|---|
| 1 | Warning | Check that the displayed log is the intended retrieval before proceeding. |
| 2 | Cancel | Closes the dialog without deleting the log. |
| 3 | OK | Deletes only the selected log after a successful authorized request. It does not unbind the Hub, delete its physical SN, or remove sub-devices. |
