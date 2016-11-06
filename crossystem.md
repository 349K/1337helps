# crossystem command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


Usage:
  crossystem [--all]
    Prints all parameters with descriptions and current values.
    If --all is specified, prints even normally hidden fields.
  crossystem [param1 [param2 [...]]]
    Prints the current value(s) of the parameter(s).
  crossystem [param1=value1] [param2=value2 [...]]]
    Sets the parameter(s) to the specified value(s).
  crossystem [param1?value1] [param2?value2 [...]]]
    Checks if the parameter(s) all contain the specified value(s).
Stops at the first error.
Valid parameters:
  arch                    Platform architecture
  backup_nvram_request    Backup the nvram somewhere at the next boot. Cleared on success.
  battery_cutoff_request  Cut off battery and shutdown on next boot.
  block_devmode           Block all use of developer mode
  clear_tpm_owner_request  Clear TPM owner on next boot
  clear_tpm_owner_done    Clear TPM owner done
  cros_debug              OS should allow debug features
  dbg_reset               Debug reset mode request (writable)
  debug_build             OS image built for debug features
  dev_boot_usb            Enable developer mode boot from USB/SD (writable)
  dev_boot_legacy         Enable developer mode boot Legacy OSes (writable)
  dev_boot_signed_only    Enable developer mode boot only from official kernels (writable)
  dev_default_boot        default boot from legacy or usb (writable)
  devsw_boot              Developer switch position at boot
  devsw_cur               Developer switch current position
  disable_dev_request     Disable virtual dev-mode on next boot
  ecfw_act                Active EC firmware
  fmap_base               Main firmware flashmap physical address
  fwb_tries               Try firmware B count (writable)
  fw_vboot2               1 if firmware was selected by vboot2 or 0 otherwise
  fwid                    Active firmware ID
  fwupdate_tries          Times to try OS firmware update (writable, inside kern_nv)
  fw_tried                Firmware tried this boot (vboot2)
  fw_try_count            Number of times to try fw_try_next (writable)
  fw_try_next             Firmware to try next (vboot2,writable)
  fw_result               Firmware result this boot (vboot2,writable)
  fw_prev_tried           Firmware tried on previous boot (vboot2)
  fw_prev_result          Firmware result of previous boot (vboot2)
  hwid                    Hardware ID
  kern_nv                 Non-volatile field for kernel use
  kernkey_vfy             Type of verification done on kernel key block
  loc_idx                 Localization index for firmware screens (writable)
  mainfw_act              Active main firmware
  mainfw_type             Active main firmware type
  nvram_cleared           Have NV settings been lost?  Write 0 to clear
  oprom_needed            Should we load the VGA Option ROM at boot?
  recovery_reason         Recovery mode reason for current boot
  recovery_request        Recovery mode request (writable)
  recovery_subcode        Recovery reason subcode (writable)
  recoverysw_boot         Recovery switch position at boot
  recoverysw_cur          Recovery switch current position
  recoverysw_ec_boot      Recovery switch position at EC boot
  ro_fwid                 Read-only firmware ID
  sw_wpsw_boot            Firmware write protect software setting enabled at boot (Baytrail only)
  tpm_attack              TPM was interrupted since this flag was cleared
  tpm_fwver               Firmware version stored in TPM
  tpm_kernver             Kernel version stored in TPM
  tpm_rebooted            TPM requesting repeated reboot (vboot2)
  try_ro_sync             try read only software sync
  tried_fwb               Tried firmware B before A this boot
  vdat_flags              Flags from VbSharedData
  vdat_lfdebug            LoadFirmware() debug data (not in print-all)
  vdat_lkdebug            LoadKernel() debug data (not in print-all)
  vdat_timers             Timer values from VbSharedData
  wipeout_request         Firmware requested factory reset (wipeout)
  wpsw_boot               Firmware write protect hardware switch position at boot
  wpsw_cur                Firmware write protect hardware switch current position

~~~
