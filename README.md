# Smokeping - Bootstrap WebGui

A modern looking smokeping webgui.

!!! This UI does not work on small screen devices

## Screenshots

<img width="1475" alt="image" src="https://github.com/svenvg93/smokeping-bootstrap/assets/4511676/297b8060-2703-4855-b1d4-d5d441c90a9f">

## Features

- Cropping graphs
- Search Functions

## Installation

### Bare metal

Replace the standaard page

```bash
 cd /etc/smokeping
 mv basepage.html basepage.html.bak
 wget https://raw.githubusercontent.com/svenvg93/smokeboot/main/basepage.html
```

### Docker

Use docker volumes to pass the into the docker container

Docker compose:

 ```bash
volumes:
- ./smokeping/basepage.html:/etc/smokeping/basepage.html
```

## Background change
Set the graphborder to no in at the top of  Presentation file to have no borders and white background on the graphs

 ```bash
graphborders = no
```

## Packet Loss Colors
To see the Packet Loss as bars in the charts set loss_background to yes in the detail section of the Presentation file 

 ```bash
loss_background = yes
```


## Acknowledgements

 - [tsumaru720/smokeping-bootstrap]([https://github.com/tsumaru720/smokeping-bootstrap])

