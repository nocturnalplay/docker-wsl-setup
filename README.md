- turn off the docker desktop system 
- shutdown the wsl in windows
> open cmd as admin

` 
wsl --shutdown
`
- list the disk contained by the wsl distro
`
wsl --list
`
- export the docker-desktop-data file to destination drive

`
wsl --export <disk file name> <destination file name>
wsl --export docker-desktop-data H:\Docker\dockerdesk.tar
`

- then unregister the docker-desktop-data 

`
wsl --unregister docker-desktop-data
`

- import the dokcer-desktop-data into the destination file 

`
wsl --import docker-desktop-data H:\Docker\desktop H:\Docker\dockerdesk.tar
`
> in windows url bar //wsl$ you can see the wsl netowrk folders
