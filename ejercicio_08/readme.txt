1-Prueba de la imagen con docker:
sudo docker run -e TELEGRAM_TOKEN=A_COMPLETAR nicopaez/telegrambot:0.0.7
I, [2021-10-18T22:40:18.155643 #1]  INFO -- : Starting bot version:0.0.7
I, [2021-10-18T22:40:18.155728 #1]  INFO -- : token is A_COMPLETAR
I, [2021-10-18T22:40:18.155776 #1]  INFO -- : Starting bot

2-kubectl create namespace arba3

3-kubectl apply -f 1-configMap.yaml -n arba3
4-kubectl apply -f 2-deployment.yaml -n arba3
