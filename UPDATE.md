<h1>Home-Lab-Server</h1>

<h2>UPDATE</h2>
For this project, I will switch to ZimaOS and plan to use a NAS to build my homelab server. This is a personal project with the goal for data privacy and protection, and saving some money from costly media subscriptions.
<br/>

<h3>What's happened and what's changed?</h3
<br/>
I was able to set up Proxmox with Docker as planned, and learned to use Portainer as well. However, without a SATA cable to connect directly to my laptop, my proxmox server was unable to read my HDD properly even with an adapter. I have decided to invest in a NAS and prioritized simplicity and decided to switch from Proxmox to ZimaOS.
<br/>
Due to low budget, this project has been postponed.

<h2>Architect for future project:</h2>

- NAS
  - Zima OS
  - Contains Docker embedded within the system
      - Frigate (security cameras control)
      - immich (photo/video storage)
