## Запуск
- Склонировать репозиторий, выполнив команду:   
`git clone https://github.com/Fr0z3Nn/alfa-bank.git`   
- Перейдя в корневую папку проекта собрать проект:    
`gradlew build`   
- Собрать докер-образ с произвольным именем, в нашем случае alfa:    
`docker image build -t alfa .`   
- Запустить контейнер с образом:   
`docker run -p 9090:9090 docker.io/library/alfa`   
***
## Endpoints
- `/api/gif`  
Возвращает гифку в зависимости от курса валют   
**Parameters**   
base: string (AED)   
**_Пример_**   
`http://localhost:9090/api/gif?base=AED`
------
- `/api/*`  
Возвращает гифку в зависимости от курса валюты (USD)    
**_Пример_**   
`http://localhost:9090/api/something`
***
