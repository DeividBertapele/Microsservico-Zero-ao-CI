# Criando e configurando um Microsserviço do Zero ao CI

- Criar o arquivo:
    - gitignore
    - Dockerfile
    - Dockerfile.prod
    - docker-compose.yaml

- Criar o requirements.txt e digita
    - django
    - gunicorn

- K8s:
    - Deployment
    - Service

- CI:
    - Build
    - Testes
    - Verificar a qualidade do código
    - Code Review
    - Políticas do repositório

- Container:
    - Registry - GCP / Privadas


-----------------------------------------------------
- Feito isso, podemos rodar no terminal do docker-compose

    - docker-compose run web django-admin startproject codeprogress .

    - docker-compose up -d

    - curl localhost:8000

- No mesmo terminal, você precisa entrar diretamente da imagem que foi instalada:

    - docker exec -it codeprogress_app bash 

 - Após entrar na execução e digita este comando para fazer migração:
        - python manage.py migrate

-----------------------------------------------------

