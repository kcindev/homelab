# homelab

<img width="2160" height="2880" alt="image" src="https://github.com/user-attachments/assets/fc389be8-46be-4750-ac1c-7a22ccfa9ea7" />

<img width="2160" height="2880" alt="image" src="https://github.com/user-attachments/assets/28cf87e7-6bce-4258-8745-08aa645c9c38" />


started my first home lab on a lenovo thinkcentre m710s

- processor: intel core i5 – 7500 (4 cores, up to 3.8ghz) 
- memory (ram): 16gb ddr4 
- gpu: intel hd 630 
- storage: ssd 250gb & hdd 500gb

Lenovo ThinkCentre M710s
└── Proxmox VE
    │
    ├── Ubuntu Server VM
    │   └── Docker
    │       ├── Portainer
    │       ├── Uptime Kuma
    │       ├── Pi-hole
    │       ├── Homarr
    │       ├── Home Assistant
    │       └── Nextcloud
    │
    ├── Kubernetes Control Plane
    ├── Kubernetes Worker 01
    ├── Kubernetes Worker 02
    │
    ├── Linux Admin/Test VM
    │
    ├── Optional Windows Server VM
    │
    └── Optional OPNsense/pfSense VM


