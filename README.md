# Gradle Masterclass

The Gradle Masterclass

DSL - Domain specific language

Groovy is a very common DSL for Gradle

It is not based on XML. XML is based on properties and values. We can’t put a logic inside XML. If you need to put a build logic you in a plugin.

Gradle scripts are regularly programming script. Is can use programming language like Groovy and Kotlin as build script. Groovy and Kotlin can run on Java Virtual Machine very well. 

Gradle can handle project of programming languages like Java, C++, Go, Groovy, Scala, JavaScript

Groovy script can be easily compared with Java code.
 
Gradle build script goes into build.gradle. Each project as it’s own build script, it will always live in the root folder of the each project In multi-project build you also have a common setting.gradle file.

## Java in Groovy
You can write Java code directly into a Gradle script. You can create inline Java methods directly into the Gradle build script without writing the main method because Gradle build file is just a Groovy script.
While Java code, semicolon “;” and braces “()” are optional. In Groovy the return statement is also optional, is such case the value of the last line will be return. Remember, this will happen only if you have declared a ‘return’ keyword in the method signature.

## Types in Groovy
def date = new Date() is equivalent to Date date = new Date(); in Java
If you do Integer i = “some string” in Groovy, it will fail, only because it is Type safe. This will however work Integer i = 10
Just remember that the type compatibility is checked at Runtime, not at compile time.

## Strings in Groovy

## Properties in Groovy
Getters and Setters in Groovy comes out of the box.

## Closures in Groovy
A closure in Groovy is an open, anonymous, block of code that can take arguments, return a value and be assigned to a variable. A closure may reference variables declared in its surrounding scope. Closures are like anonymous methods in Java. 

## Gradle task
Projects created with java-library do not have main() methods.
User defined custom tasks go under Tasks > other > myTask
Gradle check task - Plugins and build authors should attach their verification tasks, such as ones that run tests, to this lifecycle task using check.dependsOn(task)

## Multi Project
The setting.gradle file is mandatory in a multi project build

## Gradle Wrapper
Gradle Wrapper - Allows you to run a Gradle tasks without requiring that Gradle be installed on your system. You can run your project using the .gradlew script.
Run Gradle ‘wrapper’ (Build Setup > wrapper) task to generate Gradle wrapper folder, jar, properties and .gradlew files

## Useful webpages
https://docs.gradle.org/current/javadoc/index.html
https://docs.gradle.org/current/userguide/base_plugin.html
https://docs.gradle.org/current/userguide/java_plugin.html
https://docs.gradle.org/current/userguide/plugin_reference.html
https://docs.gradle.org/current/userguide/declaring_repositories.html
https://docs.gradle.org/current/userguide/declaring_dependencies.html

