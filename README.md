<h1>Home-Lab-Server</h1>

<h2>Description</h2>
For this project, I use Proxmox and an old laptop to build my homelab server. This is a personal project with the goal for data privacy and protection, and saving some money from costly media subscriptions.
<br />

<h2>Equipment and Utilities used</h2>

<li> Ventoy USB </li>
<li> Old laptop </li>
<li> Main laptop (used to configure and maintain proxmox) </li>
<i> e-thernet cable </i>
<i> e-thernet to USB-C converter
<i> HDD (seagate iron wolf) </i>

<h2>Environments Used </h2>

<li> Proxmox </li>
<li> Docker </li>
<li> Web browser from another device (in this case—my main laptop) </li>

<h2>Architect for project:</h2>

- Hardware
  - Proxmox (host OS)
    - VM with Ubuntu (for NAS)
      - Docker (container)
        - File storage (Pending)
        - immich (photo/video storage)
