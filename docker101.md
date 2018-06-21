* docker tem imagens e containers. as imagens são as máquinas, ambientes, etc. Os containers são instâncias das imagens

* para ver as imagens
docker images

* para pegar uma imagem (o docker hub em várias)
docker pull nomeDaImagem

* para apagar uma imagem
docker rmi nomeDaImagem

* para criar um container a partir de uma imagem. cada vezz que você  roda este comando será criado um container
docker run -it nomeDaImagem

* para usar um container que você  criou antes
docker container start idDoContainer #deixa rodando e cai fora
docker container start -i idDoContainer #deixa rodando interativo

* para ver os container
docker ps -a

* para apagar um container
docker rm idDoContainer

* para rodar um comando em container
docker exec idCoContainer comando
exemplo *docker exec 9a7dc7a5897f /myseq.sh 12*
myseq.sh
	#!/bin/sh    
	myseq()      
	{            
	 seq $1 -2 1 
	}            
	myseq $@     

