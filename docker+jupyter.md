To run a notebook without downloading the whole internet

`docker pull slarson/scipy-notebook`

`docker run -d -p 8888:8888 --user root -e GRANT_SUDO=yes <Conatainer Id pulled above>`
