---
tags: 
type: reference
time created: 26-08-2024
last modified: 26-08-2024
---

- Docker components
	- Client
	- Server
	- Image: Template
	- Container: Instance
	- Registries: Kho image
- Docker image
	- Tải từ Docker Hub
	- Tự tạo Dockerfile và build
- Quá trình đóng gói app
	- Viết code và dependencíe
	- Tạo dockerfile
	- Build image từ dockerfile
	- Đẩy image lên registry
	- Chạy container từ image
- Dockerfile syntax
```dockerfile
FROM <image_name:version> build image on top of existing image from Docker Hub
ARG <variable_name>=<value> define a variable to use during build image process
ENV <variable_name> <value> define a variable to use in running process inside container
RUN <command> run a Linux command
USER <username> define the user will run the process inside container, default is root
COPY <local path> <container path> copy files from local to container
CMD [<command>] define the command that launch the process within container
```
- Build image 
```bash
docker image build -t <image-name>:<tag> <path> #-t = tag
```
- Run image
	- Option
		- -d: Background (detached)
		- -p: Map port của container với port của host (port)
		- -it: Vào môi trường container (interactive)
		- -rm: Tự động xóa container sau khi thoát (remove)
```bash
docker container run <options> <image-name>
```
- Access container
```bash
docker exec -it <container-name> <command>
```