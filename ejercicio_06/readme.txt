levantar el proy. con:
* docker-compose up --scale password-api=2
* luego se puede probar con http://localhost:8080/health

NOTA: para que atendieran diferentes instancias, tuve que escalar mas, por ej con 5 instancias, sino siempre me atendia la misma instancia los llamados
