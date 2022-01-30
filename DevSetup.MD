pip3 install awscli
aws configure --profile localstack



abdi@Abdis-MacBook-Pro LogViewer % aws --profile localstack --endpoint-url=http://localhost:4566 s3 ls /               2022-01-30 14:36:02 ayusuf
abdi@Abdis-MacBook-Pro LogViewer % aws --profile localstack --endpoint-url=http://localhost:4566 s3 ls s3://ayusuf/
abdi@Abdis-MacBook-Pro LogViewer % s3 cp docker-compose.yml s3://ayusuf/    
zsh: command not found: s3
abdi@Abdis-MacBook-Pro LogViewer %  aws --profile localstack --endpoint-url=http://localhost:4566 s3 cp docker-compose.yml s3://ayusuf/
upload: ./docker-compose.yml to s3://ayusuf/docker-compose.yml    
abdi@Abdis-MacBook-Pro LogViewer % aws --profile localstack --endpoint-url=http://localhost:4566 s3 ls s3://ayusuf/2022-01-30 14:37:12        820 docker-compose.yml
abdi@Abdis-MacBook-Pro LogViewer %  aws --profile localstack --endpoint-url=http://localhost:4566 s3 cp logdata/log-123.log.txt s3://ayusuf/ 
upload: logdata/log-123.log.txt to s3://ayusuf/log-123.log.txt
abdi@Abdis-MacBook-Pro LogViewer %  aws --profile localstack --endpoint-url=http://localhost:4566 s3 cp logdata/log-123.log.txt s3://ayusuf/
upload: logdata/log-123.log.txt to s3://ayusuf/log-123.log.txt
abdi@Abdis-MacBook-Pro LogViewer %  aws --profile localstack --endpoint-url=http://localhost:4566 s3 cp logdata/log-123.log.txt s3://ayusuf/
upload: logdata/log-123.log.txt to s3://ayusuf/log-123.log.txt 




# To start up project:

$ docker-compose up
