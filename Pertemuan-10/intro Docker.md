# Intro Docker Engine  in instance EC2 AWS

1. Install based Docker Documentation (https://docs.docker.com/engine/install/ubuntu/)
   1. uninstall old version docker sudo apt remove $(dpkg --get-selections docker.io docker-compose docker-compose-v2 docker-doc podman-docker containerd runc | cut -f1)
   2. install docker
   - sudo apt-get update && sudo apt-get upgrade
   - add sertificate Repo sudo apt install ca-certificates curl sudo install -m 0755 -d /etc/apt/keyrings sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc sudo chmod a+r /etc/apt/keyrings/docker.asc
   - add Docker repository to APT sudo tee /etc/apt/sources.list.d/docker.sources <<EOF Types: deb URIs: https://download.docker.com/linux/ubuntu Suites: 
   Unable to render expression.$(. /etc/os-release &amp;&amp; echo "${UBUNTU_CODENAME:-$VERSION_CODENAME}") Components: stable Architectures: $(dpkg --print-architecture) Signed-By: /etc/apt/keyrings/docker.asc EOF
   - Update OS sudo apt update
   - Install the docker engine sudo apt install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
   - cek Installation sudo systemctl status docker
   ![alt text](image.png)

2. Registrasi Docker Hub
- URL Docker Hub (https://app.docker.com/accounts/ochakhosyyatillah)
- Continue with Github
![alt text](image-1.png)

3. Create Repository for Docker
- Klik Menu -> Hub -> Repositories
- Klik Button New Repositories
- isi nama repository dengan compro-2388010036 dan deskripsi Web App Statis Compro
- Visibility Public
- Pilih Create
![alt text](image-2.png)

4. Create token access
- Klik Profile -> Settings -> personal access tokens
- klik generate new token
- isi deskripsi
- expire date
![alt text](image-3.png)

![alt text](image-4.png)

Create Projek di local

5. buat folder compro_2388010036
- masukkan file index.html
- buat Dockerfile dengan isi sebagai berikut FROM nginx:alpine COPY index.html /usr/share/nginx/html/- - index.html EXPOSE 80
6. Push projek ke github
![alt text](image-5.png)