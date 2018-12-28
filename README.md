# NFE PHP com docker

Estou pressupondo que você está em ambiente linux (Ubuntu ;) com Docker e Docker compose instalados e funcionando.

** Passos **

- Clone o repositorio git@github.com:nfephp-org/sped-nfe.git
- Baixe as dependências (Pasta vendor) via docker. Execute o comando abaixo dentro da pasta do sped-nfe
    `docker run --rm -it --volume $(pwd):/app prooph/composer:7.1 install -o --prefer-dist`
- Copie todos os arquivos desses repositório e coloque na pasta sped-nfe
- Execute: `docker-compose up --build`
- Verifique se seus container estão funcionando:  `docker ps`
- Acesse: http://localhost:8000