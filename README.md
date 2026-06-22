# homelab

<img width="2160" height="2880" alt="image" src="https://github.com/user-attachments/assets/fc389be8-46be-4750-ac1c-7a22ccfa9ea7" />

<img width="2160" height="2880" alt="image" src="https://github.com/user-attachments/assets/28cf87e7-6bce-4258-8745-08aa645c9c38" />


started my first home lab on a lenovo thinkcentre m710s

- processor: intel core i5 – 7500 (4 cores, up to 3.8ghz) 
- memory (ram): 16gb ddr4 
- gpu: intel hd 630 
- storage: ssd 250gb & hdd 500gb

this home lab was built as a single ubuntu server host running docker containers and a small number of host-level services. it currently provides:

- container management
- service monitoring and discord alerts
- network-wide dns filtering
- smb file sharing
- a self-hosted dashboard
- host resource monitoring
- home automation
- private cloud file storage
- persistent storage and nightly backups

the home lab follows a predictable directory structure:

```text
/srv/
├── docker/
│   ├── portainer/
│   ├── uptime-kuma/
│   ├── pihole/
│   ├── homarr/
│   ├── dashdot/
│   ├── homeassistant/
│   └── nextcloud/
└── storage/
    ├── shared/
    └── nextcloud/
```

| path | purpose |
|---|---|
| `/srv/docker` | compose files, application data, databases, and `.env` files |
| `/srv/storage` | persistent data on the 500 gb hdd |
| `/srv/storage/shared` | samba share |
| `/srv/storage/nextcloud` | nextcloud personal files |


---

| service |
|---|
| portainer |
| uptime kuma |
| pi-hole |
| dns |
| samba |
| homarr |
| dash |
| home assistant |
| nextcloud |
| mariadb |
| redis |


---

planning on switching to proxmox ve soon

```text
proxmox ve
│
├── ubuntu server vm
│   └── existing docker services
│       ├── portainer
│       ├── uptime Kuma
│       ├── pi-hole
│       ├── homarr
│       ├── dash. or replacement monitoring tool
│       ├── home assistant
│       └── nextcloud
│
├── kubernetes vm
├── linux administration vm
├── windows server vm
└── opnsense/pfsense networking vm
```


