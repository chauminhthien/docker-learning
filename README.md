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
  `docker run --name {container_name} -p {host_port}:{container_port} -v {/host_path}:{/container_path} -it {image_name} /bin/bash`
  `docker run -it --name {Container name} -h {hostname} {images}`

  docker run -it --network {name net work}
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

## Thực thi cách hàm trong container đang chay
  ```
    `docker exce {name_container} {lệnh}`
    vd: `docker exce U1 ls -a`
  ```

## Tao Images mới
  `docker commit {tên container} image:tag`

## Lưu images thành file
  `docker save --output {filename.tar} {id image}`

## Load image từ file có sẳn
  `docker load -i {duong dan tới file}`

## Sửa name và tag image
  `docker tag {id} {newName:newTag}`

## Cách chia sẽ thư muc máy host với container
  `docker run -it -v {path máy host}:{path container}`

## Cách chia sẽ thư mục từ container đang chay
  `docker run -it --volumes-form {name container đang chay} {name image}`

## Xem volume có trong docker
  `docker volume ls`

## Tạo volume cho docker
  `docker volume create {name}`

## Kiểm tra thông số volume
  `docker volume inspect {name}`

## Tạo volume cho docker ánh xa5 tới thư mục máy host
  `docker volume create --opt devive={path máy host} --opt type=none --opt o=bind {name volume}`

## Xoá volume
`docker volume rm -f {name}`


## Gán volume khi run docker
`docker run -it --mount source={name volume},taget={path tren images} {name image}`


## Xem danh sách network trong docker
`docker network ls`

## Xem chi tiết network trong docker
```
  docker network inspect {name network}
  `Containers` chính là danh sách các container connet tới
  networt `bridge` mặt định được connect khi run image
```


## Xem container đang connet tới network nào
  `docker inspect {name container}`


## Tạo mới một network
  `docker network create --driver {name driver network} {name network new}`

## Xoá network
  `docker network rm {name}`

## Kiêm tra lich sử của image
  `docker images history {id/name image}`

## Kiêm tra log container
  `docker logs {name container}`

## Kiêm tra log container và theo dõi
  `docker logs -f {name container}`








# ==== Một số lỗi có thể gặp ====

## không cái được package
  [Link fix](https://unix.stackexchange.com/questions/336392/e-unable-to-locate-package-vim-on-debian-jessie-simplified-docker-container)