<div align="center">
  <img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%" height="4" />
  <br/><br/>

  <p>
    <img src="https://img.shields.io/badge/NODE-mrizkymxx--core-0d1117?style=flat-square&logo=gnu-bash&logoColor=00FF9C" alt="Node ID" />
    <img src="https://img.shields.io/badge/STATUS-OPERATIONAL-00FF9C?style=flat-square&logo=opsgenie&logoColor=00FF9C" alt="Status" />
    <img src="https://img.shields.io/badge/UPTIME-99.98%25-00F5FF?style=flat-square" alt="Uptime" />
    <img src="https://img.shields.io/badge/RTT-12ms-00FF9C?style=flat-square" alt="Latency" />
    <img src="https://img.shields.io/badge/LOC-Jepara%2C_ID-00F5FF?style=flat-square" alt="Location" />
  </p>

  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=00FF9C&background=0D111700&center=true&vCenter=true&width=450&height=50&lines=IT+Support;SysAdmin;PowerShell+Automation;Network+Ops" alt="Terminal Typing Telemetry" />
  <br/>

  <img src="https://stuff.charm.sh/vhs/examples/neofetch_3.gif" alt="Terminal Session Neofetch" width="550" />
  <br/><br/>

  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=powershell,bash,linux,windows,docker,git,python,azure,aws,regex,debian,ubuntu,nginx,cloudflare&perline=7&theme=dark" alt="Technical Stack Icons" />
  </a>
  <br/><br/>

  <img src="https://github-readme-stats.shion.dev/api?username=mrizkymxx&show_icons=true&theme=tokyonight&bg_color=0d1117&hide_border=true" height="150" alt="GitHub Metrics" />
  <img src="https://streak-stats.demolab.com/?user=mrizkymxx&theme=tokyonight&background=0d1117&hide_border=true" height="150" alt="Deployment Streak" />
  <br/><br/>

  <img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%" height="4" />
</div>

```
================================================================================
HOST: mrizkymxx-node01    OS: Win11Pro / Debian 12    KERNEL: 6.1.0-lts
TARGET: IT Support / Systems Support / IT Operations    SECURITY: Hardened
LOC: Jepara, Central Java, ID                           TIMEZONE: UTC+7 (WIB)
================================================================================
```

## [01] SYSTEM_MANIFEST & TECHNICAL_SUMMARY

Systems support specialist with production floor and field deployment record. Core focuses on edge network fault tolerance under harsh physical conditions, hardware diagnostic protocols, peripheral firmware/interface troubleshooting (ESC/POS thermal printers, industrial RS-232/USB barcode scanners), and zero-touch workstation automation. Unattended scripting over manual triage.

```
[SYS] Windows 10/11 Pro Endpoint Provisioning & Hardening
[NET] 802.1Q VLANs, DHCP/DNS Failover, MTU Optimization, Wireshark Analysis
[PER] ESC/POS Protocol, Serial/USB Communication, Kiosk Watchdogs
[OPS] PowerShell 7+ Automation, WMI/CIM Event Traps, Bash Maintenance
```

---

## [02] TECHNICAL_COMPETENCIES_MATRIX

| Domain | Production Implementations |
| :--- | :--- |
| **Operating Systems** | Windows 10/11 Pro (imaging, sysprep, GPO, registry hardening), Linux/Debian (systemd, headless administration). |
| **Networking & Protocols** | IPv4 subnetting, VLAN tagging (802.1Q), DHCP/DNS triage, routing tables, TCP/UDP packet analysis via Wireshark, ARP/MTU debugging. |
| **Hardware & Peripherals** | Industrial touch terminals, ESC/POS thermal printers, RS-232/USB-to-Serial converters, optical/laser barcode scanners, crimping (T568B). |
| **Scripting & Automation** | PowerShell (WMI/CIM, Event Log parsing, process supervisors), Bash, Windows Batch. |
| **Databases & Services** | PostgreSQL (PostGIS geospatial queries), Supabase (Auth, Realtime, Storage), Firestore, Nginx reverse proxy. |
| **IT Operations Discipline** | Root-cause analysis (RCA), disaster recovery procedures, incident response runbooks, inventory lifecycle auditing. |

<p align="center">
  <img src="https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white" alt="PowerShell" />
  <img src="https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white" alt="Bash" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux" />
  <img src="https://img.shields.io/badge/Windows_Server-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows Server" />
  <img src="https://img.shields.io/badge/Cisco-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white" alt="Cisco" />
  <img src="https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white" alt="Wireshark" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
</p>

---

## [03] FIELD_DEPLOYMENTS & RUNBOOKS

### 1. BSMCartonBox — Factory Production & Inventory Operations
`Stack: Next.js, Firebase Firestore, PWA, ESC/POS Barcode Scanners, Industrial Touch Terminals`

Shop-floor tracking system operating inside corrugated box manufacturing plant. Conditions: airborne dust, motor EMI, thermal swings, spotty 2.4GHz WLAN.

* **Edge Resilience:** Service-worker caching + IndexedDB write queues. Corrugator operators log output without data loss during AP roaming handoffs.
* **Hardware Diagnostics:** Resolved USB HID scanner lockups from line-voltage drops. Pinned USB selective suspend flags across all floor clients.
* **Data Integrity:** Client mutation locks and debouncing eliminated duplicate records from operator double-taps on resistive screens.

<details>
<summary><b>[RUNBOOK-01] Industrial Terminal Freeze & Firestore Sync Stall</b></summary>

```
SYMPTOM: Terminal 03 on Corrugator Line shows stale queue.
         Barcode scans emit hardware beep but input field remains empty.
         Firestore local buffer growing unbounded.
```

1. **Physical & Power Rail Audit:**
   Verify USB 5V rail on terminal hub. Check scanner cable for pinch damage along machine chassis.
2. **Peripheral State Check (PowerShell):**
   ```powershell
   Get-PnpDevice -PresentOnly | Where-Object { $_.FriendlyName -match "POS|Barcode|HID" } | Select-Object Status, Class, FriendlyName, InstanceId
   ```
   *Action:* If status returns `Error` or `Degraded`, cycle USB root hub power state.
3. **Application State Verification:**
   Query Chrome kiosk remote debugging port:
   ```bash
   curl -s http://127.0.0.1:9222/json | grep -i "devtoolsFrontendUrl"
   ```
4. **Storage Quota & Index Audit:**
   Execute in devtools context:
   ```javascript
   navigator.storage.estimate().then(est => console.log((est.usage / est.quota * 100).toFixed(2) + "% used"));
   ```
   *Action:* Purge stale log chunks if usage exceeds 90%.
5. **Network MTU & Fragmentation Check:**
   Ping factory gateway with Don't Fragment flag:
   ```cmd
   ping 192.168.10.1 -f -l 1472
   ```
6. **Supervisor Recovery:**
   Relaunch kiosk container via watchdog:
   ```powershell
   Stop-Process -Name "chrome" -Force; Start-Process "C:\Kiosk\launch-line2.bat"
   ```
</details>

---

### 2. Q-Premium Queue — On-Site Kiosk, Thermal Printing & Realtime Sync
`Stack: Flutter, Supabase Realtime (PostgreSQL CDC/WebSockets), ESC/POS Thermal Printers, Serial/USB`

On-premise queue management kiosk with automated ticket cutting, counter display paging, and mobile sync.

* **Peripheral Protocol Control:** Interfaced directly with ESC/POS hardware over raw endpoints (`COM`/`usblp`). Constructed custom hex payloads for raster graphics, barcode printing, and cash drawer kick/paper cut routines (`0x1D 0x56 0x41`).
* **Network Segmentation:** Segregated kiosk terminals and counter display hardware into isolated `VLAN 30`. Denied ingress from public client subnet via router ACLs.
* **Process Watchdog:** Implemented automated restart supervisor. Detects hung UI threads, dropped WebSockets, or frozen print buffers; performs warm process recovery in under 3 seconds.

<details>
<summary><b>[RUNBOOK-02] ESC/POS Thermal Printer Lockup & Buffer Overflow</b></summary>

```
SYMPTOM: Ticket dispenser outputs partial lines, prints endless blank feed,
         or flashes red error LED (buffer overflow / cutter blade jam).
         Counter display displays WebSocket disconnect status.
```

1. **Mechanical & Cutter Clear:**
   Open chassis. Clear jammed paper bits from guillotine blade. Cycle main power switch to restore blade home position.
2. **Buffer Flush via Direct Serial Hex Payload:**
   Send `ESC @` (`0x1B 0x40`) hardware reset sequence directly to interface:
   ```powershell
   $port = New-Object System.IO.Ports.SerialPort "COM3", 9600, [System.IO.Ports.Parity]::None, 8, [System.IO.Ports.StopBits]::One
   $port.Open()
   $port.Write([byte[]](0x1B, 0x40), 0, 2)
   $port.Close()
   ```
3. **Print Spooler Reset (Windows Client):**
   ```powershell
   Stop-Service -Name Spooler -Force
   Remove-Item -Path "$env:SystemRoot\System32\spool\PRINTERS\*" -Force
   Start-Service -Name Spooler
   ```
4. **WebSocket Endpoint Connectivity Test:**
   ```powershell
   Test-NetConnection -ComputerName "db.lan" -Port 5432
   Get-NetTCPConnection -RemotePort 443 | Where-Object State -eq "Established"
   ```
5. **Hardware Self-Test:**
   Hold feed button during power switch engagement. Verify DIP switch configuration matches OS baud settings (9600 vs 115200 bps).
</details>

---

### 3. Lapor Desa Rau — Citizen Ticketing & Field Dispatch Platform
`Stack: Next.js, PostgreSQL / PostGIS, Leaflet, Supabase Storage, Nginx`

Municipal incident reporting platform with spatial boundary enforcement for public infrastructure remediation and village administration.

* **Rural Cellular Bandwidth Optimization:** Field crews upload work orders over congested 3G/HSPA+ networks. Enforced client-side canvas rasterization (downscaled to 1280px WebP, 75% quality). Payload size dropped from 6MB to 350KB, reducing transmission dropouts by 94%.
* **Spatial Boundaries:** Tuned PostGIS tables with `GIST` indexes. Verified report coordinates against administrative boundaries via `ST_Contains` to reject out-of-jurisdiction submissions prior to storage writes.
* **Operational Backups:** Automated rolling database dumps and object bucket sync via cron jobs with Slack webhook reporting on non-zero exit codes.

<details>
<summary><b>[RUNBOOK-03] Mobile Dispatch Upload Failures & Geofence Rejections</b></summary>

```
SYMPTOM: Field devices encounter HTTP 413 / HTTP 504 on photo submission.
         Valid internal tickets rejected with "Outside service zone" warning.
```

1. **PostGIS Coordinate Axis Alignment Audit:**
   Verify coordinate ordering. Device GPS emits Latitude/Longitude (`Y, X`), whereas PostGIS `ST_MakePoint` requires Longitude/Latitude (`X, Y`):
   ```sql
   SELECT id, name 
   FROM desa_boundaries 
   WHERE ST_Contains(geom, ST_SetSRID(ST_MakePoint(110.6872, -6.5912), 4326));
   ```
2. **Reverse Proxy Ingestion Size Verification:**
   Inspect Nginx payload ceiling configuration:
   ```bash
   grep -rn "client_max_body_size" /etc/nginx/
   # Required setting: client_max_body_size 10M;
   nginx -t && systemctl reload nginx
   ```
3. **Storage Mount Capacity Check:**
   ```bash
   df -h /var/lib/docker/volumes/
   ```
4. **Log Inspection:**
   ```bash
   tail -n 100 /var/log/nginx/error.log | grep -E "413|client intended to send too large body"
   ```
</details>

---

### 4. IT Automation & Systems Diagnostics Toolkit
`Stack: PowerShell 7+, Windows Command Shell (Batch), Bash, WMI/CIM, Sysinternals`

Modular diagnostic repository designed for unattended fleet provisioning, interface troubleshooting, and rapid hardware audits across commercial enterprise endpoints.

* **Zero-Touch Provisioning:** Modular scripts managing initial machine setup: silent package deployment (`winget`/`msiexec`), registry hardening, telemetry suppression, firewall profile activation, and local user creation.
* **Diagnostic Utilities:** One-click scripts for service-desk staff: flushes network stacks, resets WINSOCK/ARP tables, purges deadlocked print queues, and extracts physical drive SMART statistics.
* **Forensic Auditing:** Automated queries extracting security audit failures (Event ID 4625), unexpected service halts (Event ID 7034), and thermal throttling triggers via `Get-WinEvent`.

<details>
<summary><b>[RUNBOOK-04] Production Endpoint Triage & Stack Reset Script</b></summary>

```powershell
<#
.SYNOPSIS
    Endpoint Rapid Remediation & Diagnostics
    Author: Muhammad Rizky (@mrizkymxx)
#>

# 1. Verify Elevation
$isAdmin = ([Security.Principal.WindowsPrincipal][Security.Principal.WindowsIdentity]::GetCurrent()).IsInRole([Security.Principal.WindowsBuiltInRole]::Administrator)
if (-not $isAdmin) {
    Write-Error "Elevated prompt required. Run as Administrator."
    exit 1
}

Write-Host "[+] Initiating Endpoint Diagnostics..." -ForegroundColor Cyan

# 2. Storage Health Check (SMART Status)
Write-Host "[+] Auditing Physical Disks:"
Get-CimInstance -ClassName MSStorageDriver_FailurePredictStatus -Namespace root\wmi | ForEach-Object {
    $drive = $_.InstanceName
    $status = if ($_.PredictFailure) { "FAILING CRITICAL" } else { "HEALTHY" }
    Write-Host "    Disk: $drive -> Status: $status" -ForegroundColor ($_.PredictFailure ? "Red" : "Green")
}

# 3. Print Spooler Deadlock Recovery
Write-Host "[+] Purging Print Spooler Deadlocks..."
Stop-Service -Name Spooler -Force -ErrorAction SilentlyContinue
$spoolDir = Join-Path $env:SystemRoot "System32\spool\PRINTERS\*"
Remove-Item -Path $spoolDir -Force -ErrorAction SilentlyContinue
Start-Service -Name Spooler
Write-Host "    Spooler restarted cleanly." -ForegroundColor Green

# 4. Network Stack Flush
Write-Host "[+] Resetting Network Interfaces & DNS Cache..."
ipconfig /flushdns | Out-Null
arp -d * 2>$null
netsh interface ip delete arpcache | Out-Null

# 5. Extract Critical Events Past 24 Hours
Write-Host "[+] Scanning Recent System Error Events (Past 24h):"
$cutOff = (Get-Date).AddDays(-1)
$events = Get-WinEvent -FilterHashtable @{
    LogName = 'System'
    Level = 2 # Error
    StartTime = $cutOff
} -MaxEvents 5 -ErrorAction SilentlyContinue

if ($events) {
    $events | Select-Object TimeCreated, Id, ProviderName, Message | Format-Table -AutoSize
} else {
    Write-Host "    No critical system error events detected." -ForegroundColor Green
}

Write-Host "[+] Remediation routine complete." -ForegroundColor Cyan
```
</details>

---

## [04] TELEMETRY_PIPELINE & ACTIVITY

<div align="center">
  <img src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg" alt="Contribution Grid Snake Activity" width="100%" />
  <br/><br/>
  <img src="https://github-readme-stats.shion.dev/api/top-langs/?username=mrizkymxx&theme=tokyonight&bg_color=0d1117&hide_border=true&layout=compact" height="150" alt="Top Languages Breakdown" />
</div>

---

## [05] TERMINAL_ENDPOINTS

```bash
# Direct Communications & Diagnostic Shell
$ ping -c 4 mrizkymxx.local
$ open mailto:mrizkymxx@gmail.com
$ curl -s https://linkedin.com/in/mrizkymxx
$ gh repo clone mrizkymxx/mrizkymxx
```

<div align="center">
  <img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%" height="4" />
  <p><b>[SYSTEM HALTED: NORMAL TERMINATION]</b></p>
</div>
