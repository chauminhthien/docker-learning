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




# ============ Một số lỗi có thể gặp ======================

## không cái được package
  [Link fix](https://unix.stackexchange.com/questions/336392/e-unable-to-locate-package-vim-on-debian-jessie-simplified-docker-container)