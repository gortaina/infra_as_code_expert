


- [ ] Configuração de região do S3, onde encontrar
- [ ] Cuidado com o arquivo de estado terraform.tfstate
- [ ] Verificar arquivos mínimos para o hello world, main.tf
- [ ] lista de comandos para rollback

Para aula-02, só o main.tf é necessários, coloque os outros arquivos noutro diretório

execução para o docker
sudo docker run -it -v $PWD:/app -w /app --entrypoint "" hashicorp/terraform:light sh

lista de comando para rollback

<br>-destrua o plano
<br>terraform destroy
<br>-saia do contêiner
<br>exit
<br>-listar os contêiner, copiar o CONTAINER ID da imagem "hashicorp/terraform:light "
<br>docker ps -l
<br>-parar o contêiner
<br>docker stop "container id"
<br>-remover o contêiner
<br>docker rm "container id"
<br>-listar os arquivos ocultos, como o do state do terraform
<br>ls -a
<br>-apagar o diretório do state do terraform
<br>sudo rm -rf .terraform/
<br> opcional, listar e depois remover a imagem desejada
docker images  
docker rmi "IMAGE ID"

