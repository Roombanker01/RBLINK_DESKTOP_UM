# Hubs and registration

The standard protection controls are ordered **Arm Stay**, **Arm Away**, then **Disarm**. They are high-impact controls: verify the Hub and use the refreshed state as confirmation.

![Hub list actions: 1 Hub List, 2 status, 3 mode, 4 company, 5 SN, 6 Add Hub, 7 sub-devices, 8 Arm Stay, 9 Arm Away, 10 Disarm, 11 details, 12 assign, 13 delete](/images/hubs/hub-list-actions.png){.manual-shot}

| No. | Control | Use and result |
|---|---|---|
| 1 | Hub List | Returns to the Hub list. |
| 2 | Status filter | Limits the list by Hub status. |
| 3 | Mode filter | Limits the list by current arm mode. |
| 4 | Company filter | Limits the list to a company. |
| 5 | SN search | Filters by Hub serial number. |
| 6 | Add Hub | Opens the registration wizard. |
| 7 | Sub-devices | Opens that Hub's sub-devices. |
| 8 | Arm Stay | Changes the selected Hub to Arm Stay. Verify the Hub and intended mode first; if the action fails, do not assume the mode changed. |
| 9 | Arm Away | Changes the selected Hub to Arm Away. Verify the Hub and intended mode first; if the action fails, do not assume the mode changed. |
| 10 | Disarm | Disarms the selected Hub. Verify the Hub and intended mode first; if the action fails, do not assume the mode changed. |
| 11 | Details | Opens the selected Hub detail. |
| 12 | Assign | Opens assignment without changing it. |
| 13 | Delete | Opens deletion confirmation. |

![Assign Hub: 1 company, 2 person, 3 cancel, 4 save](/images/hubs/hub-assign-modal.png){.manual-shot}

| No. | Control | Use and result |
|---|---|---|
| 1 | Company | Select the target company. |
| 2 | Assign to person | Search/select an eligible person after choosing a company. |
| 3 | Cancel | Closes without changing the assignment. |
| 4 | Save | Saves the assignment when authorized; failure leaves the current assignment unchanged. |

![Delete Hub confirmation: 1 consequence, 2 cancel, 3 confirm](/images/hubs/hub-delete-confirm.png){.manual-shot}

| No. | Control | Use and risk |
|---|---|---|
| 1 | Unbinding consequence | Verify the Hub: deletion removes personal/company bindings; its physical SN record remains. |
| 2 | Cancel | Closes without deletion. |
| 3 | Confirm | Authorized deletion makes the Hub unavailable in PC until rebound. |

![Add Hub step 1: 1 Power and Connect, 2 Ready Continue, 3 Close](/images/hubs/hub-add-step-1.png){.manual-shot}

| No. | Step 1 control | Prerequisite, action, result, failure or permission |
|---|---|---|
| 1 | Power & Connect | Power the Hub and establish its required Ethernet or LTE connection before continuing. |
| 2 | Ready - Continue | Moves to SN entry; it does not add or bind a Hub. |
| 3 | Close | Leaves the wizard without adding a Hub. |

![Add Hub step 2: 1 Hub SN, 2 Back, 3 Next, 4 Close](/images/hubs/hub-add-step-2.png){.manual-shot}

| No. | Step 2 control | Prerequisite, action, result, failure or permission |
|---|---|---|
| 1 | Hub SN | Enter the SN (serial number) printed on the device label. Only letters and numbers are allowed; an empty or invalid SN does not advance. |
| 2 | Back | Returns to Power & Connect and preserves the wizard rather than binding a Hub. |
| 3 | Next | Validates the SN and opens company ownership selection. |
| 4 | Close | Cancels the wizard without creating a binding. |

![Add Hub step 3: 1 search, 2 No Company, 3 company option, 4 Load more, 5 Confirm Add Hub](/images/hubs/hub-add-step-3.png){.manual-shot}

| No. | Step 3 control | Prerequisite, action, result, failure or permission |
|---|---|---|
| 1 | Company search | Search the selectable companies for the validated SN. |
| 2 | No Company | Clears the selection. The page then hides Confirm Add Hub, so no binding can be made. |
| 3 | Company option | Select the intended company; verify ownership before continuing. |
| 4 | Load more | Loads the next available company page. If a company search request fails, the dropdown shows Retry; retry preserves the wizard and does not bind a Hub. |
| 5 | Confirm Add Hub | Available after a company is selected. It is a high-impact binding action. Success binds the Hub to the selected company; a validation error or failure leaves the wizard available to correct or retry. |

**Deletion risk.** Deleting a Hub removes its personal and company bindings; it is not visible in the PC until rebound. The physical SN record is retained and is not physically deleted.
