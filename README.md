version: 0.2

phases:
install:
runtime-versions:
java: corretto11

build:
commands:
- mvn clean install

post_build:
commands:
- echo "Build complete"

artifacts:
files:
- target/*.jar
