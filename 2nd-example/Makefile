all: compile

compile:
	java -jar ../jflex-full-1.9.1.jar scanner.flex
	java -jar ../java-cup-11b.jar -interface -parser Parser parser.cup
	javac -cp ../java-cup-11b-runtime.jar *.java

execute:
	java -cp ../java-cup-11b-runtime.jar:. Main

clean:
	rm -f *.class *~
