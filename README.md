# DockerAndKubernetes
 Curso de Docker - Docker & Kubernetes: The Practical Guide

# Comands
* docker run image_name;  Caso a imagem de node não esteja instalada, ela é baixada do docker hub. Exemplo: 

* docker ps -a : Mostra todas as imagens disponíveis. 

* docker run -it node: Permite rodar o container expondo-o. 

* docker build Constroi uma imagem baseado no arquivo docker

* docker run -p 3000:80 d3510170aed8: Mapeia a porta 3000 da máquina, que roda o container, para a porta 80 do computador. Dessaforma é possível acessar a aplicação na porta 3000.

* docker start container_name : inicia um container sem o recriar.

* docker run -it container_name : incia o container apartir da imagem de modo interativo

* docker start -ai container_name : inicia o container de modo interativo

* docker images: lista todas as imagens

* docker rmi sha_image: remove uma imagem

* docker image prune: remove todas as imagens

* docker image inspect image_id: permite verificar alguns detalhes da imagem

* docker run -p 3000:80 -d -v feedback:/app/feedback --name feedback-container-volume --rm feedback-volume : cria um container com mapeamento da porta 80 para a 3000 com um named volume que manterá os arquivos salvos mesmo quando o container for removido. Além disso, esse container também será removido assim que for parado

* docker run -p 3000:80 -d -v feedback:/app/feedback -v "C:\Users\word2\Documents\Docker\data-volumes-01-starting-setup:/app" -v /app/node_modules --name feedback-container-volume --rm feedback-volume