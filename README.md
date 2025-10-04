#  System Resource Monitoring using Netdata

##  Project Overview
This project demonstrates how to monitor system resources in real time using **Netdata**, an open-source, lightweight monitoring tool.  
Netdata provides live metrics for CPU, memory, disk, network, and containers through a visual web dashboard.

---

##  Setup Instructions

### 1. Run Netdata with Docker
```bash
docker run -d --name=netdata \
  -p 19999:19999 \
  --cap-add SYS_PTRACE \
  --security-opt apparmor=unconfined \
  netdata/netdata
````

### 2. Access the Dashboard

* Open your browser and go to:
  👉 [http://localhost:19999](http://localhost:19999)

You’ll see real-time metrics for:

* CPU usage
* Memory utilization
* Disk I/O
* Network traffic
* Running Docker containers

---

## 🧾 Viewing Logs

If you want to check Netdata logs inside the container:

```bash
docker exec -it netdata bash
cd /var/log/netdata
ls
```

---

## ⚙️ Stopping Netdata

To stop and remove the container:

```bash
docker stop netdata
docker rm netdata
```

---

##  Key Features

* Real-time system performance monitoring
* Beautiful web-based dashboard
* Zero-configuration installation
* Works with containers, VMs, and bare-metal systems

---


<img width="1835" height="372" alt="image" src="https://github.com/user-attachments/assets/bbc11c74-7f12-4da2-b929-4956338dd97e" /><br>
<br>
<br>
<img width="1919" height="972" alt="image" src="https://github.com/user-attachments/assets/eef4e0df-d873-4615-a66c-8aadd59333d6" /><br>
<br>
<br>
<img width="1915" height="921" alt="image" src="https://github.com/user-attachments/assets/2c1f36a3-3f9b-4d9f-8a55-1284421179da" /><br>
<br>
<br>
<img width="1903" height="912" alt="image" src="https://github.com/user-attachments/assets/daf94d24-ed61-4db9-9776-f91e7c3ef643" />
<br>
<br>
<br>
<img width="1916" height="968" alt="image" src="https://github.com/user-attachments/assets/e66c7abd-278a-4e23-8bd7-2abeec1c9e71" />

