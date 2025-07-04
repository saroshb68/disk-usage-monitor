# 🧠 Linux Disk Usage Monitor Script

A simple Bash script that monitors disk space usage on Linux systems and sends an alert email if any partition exceeds a defined threshold (default: 80%).

## 📌 Features
- Checks disk space using `df -h`
- Filters partitions above 80%
- Sends email notifications for critical usage
- Can be automated via `cron`

## 🛠 Technologies Used
- Bash
- df, awk, grep
- mail / sendmail (for alerting)
- crontab (for scheduling)

## 📂 How to Use
1. Clone or download the script.
2. Make it executable:
```bash
chmod +x disk_monitor.sh
```
3. Edit threshold/email inside the script as needed.
4. Run manually or via cron:
```bash
*/30 * * * * /path/to/disk_monitor.sh
```

## ✅ Sample Output
```
Warning: /dev/sda1 has reached 91% usage
Please take action.
```

## 📧 Alerts
Email subject: `Disk Space Alert`
