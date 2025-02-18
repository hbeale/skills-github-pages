---
title: "Dynamic access to data on servers"
date: 2025-02-18
---

# Dynamic access to data on servers

Instructions for mounting a local drive are here: https://github.com/UCSC-Treehouse/holly_beale_lab_notebook/blob/main/analysis_records/mount_server_volume_to_local_drive.md

You can also run your code on open stack through the browser. If you want to run R code, I prefer RStudio server (https://posit.co/download/rstudio-server/) to Rstudio docker (instrux below) because of permission issues with Docker. Full disclosure; I've only run RStudio server on mustard, not openstack.


## Use RStudio docker on an open stack computer

create /home/ubuntu/.rstudio_env_file, e.g. 
```
PASSWORD=your_password_here
```

```
docker run --rm -it --env-file ~/.rstudio_env_file -p 18845:8787 --entrypoint=/bin/bash -v /mnt:/mnt rocker/verse
```

then run:
`/init`

connect at
http://10.50.100.58:18845/

username is rstudio; password is from your rstudio_env_file
