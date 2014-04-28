hello-world
===========

Hello World

# Compilando os fontes
javac Greetings.java 
javac GreetingsService.java 
javac App.java 

# Executando a classe App
java App Guest

# Empacotando a aplicação
jar -cf system.jar Greetings.class GreetingsService.class App.class

# Executando a classe App do pacote system.jar
java -classpath system.jar App Guest

# Reempacotando a aplicação com arquivo de manifesto
jar -cfm system.jar manifest.txt Greetings.class GreetingsService.class App.class

# Executando a aplicação empacotada
java -jar system.jar Guest
