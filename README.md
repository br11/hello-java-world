hello-world
===========

Hello World em Java

### Compilando os fontes
javac Greetings.java 
javac GreetingsService.java 
javac App.java 

### Executando a classe App
java App Guest

### Empacotando a aplicação
jar -cf app.jar Greetings.class GreetingsService.class App.class

### Executando a classe App do pacote system.jar
java -classpath app.jar App Guest

### Reempacotando a aplicação com arquivo de manifesto
jar -cfm app.jar manifest.txt Greetings.class GreetingsService.class App.class

### Executando a aplicação empacotada
java -jar app.jar Guest
