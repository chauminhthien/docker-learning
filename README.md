[Link hub search docker](https://hub.docker.com).

## Liệt kê danh sách images đang có
  `docker images`

## Xoá 1 image
  `docker image rm {name/id_image}`

## Tìm kiếm images tren hub docker
  `docker search {ten_tim_kiem}`

## Cách run image
```
  `docker run -it {name/id_iamge}`
  `docker run --name {container_name} -p {host_port}:{container_port} -v {/host_path}:{/container_path} -it {image_name} /bin/bash` \n
  `docker run -it --name {Container name} -h {hostname} {images}` \n
```
## Liệt kê các container đang chạy
  `docker ps`

## Liệt kê các container đã tắt
  `docker ps -a`

## Xóa một container
  `docker rm -f {container_id/name}`

## Đổi tên một container
  `docker rename {old_container_name} {new_container_name}`

## Commit các thay đổi trên container và image
  `docker commit -m "message" {container_name} {image_name}`

## Start lại container
  `docker start {id}`

## Stop lại container
  `docker stop {id}`

## Đi vào cửa sổ cmd docker
  `docker attach -i {id}`


## Thoát cửa sổ cmd của container
  `Tổ hợp phim ctrl + p + q`
