# DockerAndKubernetes
 Curso de Docker - Docker & Kubernetes: The Practical Guide

# Comands
* docker run image_name;  Caso a imagem de node não esteja instalada, ela é baixada do docker hub. Exemplo: 

* docker ps -a : Mostra todas as imagens disponíveis. 

* docker run -it node: Permite rodar o container expondo-o. 

* docker build Constroi uma imagem baseado no arquivo docker

* docker run -p 3000:80 d3510170aed8: Mapeia a porta 3000 da máquina, que roda o container, para a porta 80 do computador. Dessaforma é possível acessar a aplicação na porta 3000.