# Metaplex-Deployer


### Upload Docker Image
TODO: Bake into build process

`aws ecr-public get-login-password --region us-east-1 | docker login --username AWS --password-stdin public.ecr.aws/k2z7t6t6`

`docker build -t metaplex-deployer .`

`docker tag metaplex-deployer:latest public.ecr.aws/k2z7t6t6/metaplex-deployer:latest`

`docker push public.ecr.aws/k2z7t6t6/metaplex-deployer:latest`
