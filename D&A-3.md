Introduction to Classes and Objects - Part 1 (Data Structures & Algorithms #3)

Comparing two robots in whatever programming language youre using you need to have two sets of information

    1st set : The properties that each robot has:
        ex. - name : "Tom" , color : "red" , weight : 30
            - function : to introduce self (introduceSelf())

        Object would be best to store this info since it is a collection of properties
        An object can represent some thing in this case, the robot Tom.

        Once you create the object you can store it as a variable and call it like any other variable.

    2nd set : ex - name : "Jerry" , color : "blue" , weight : 40
                 - function : introduceSelf()

A class is like a blueprint from which you can make objects.

For the two objects a class that would be the blueprint for them would be something like this : - name : - color : - weight : + introduceSelf()

Written in Java:

Robot r1 = new Robot();
r1.name = "Tom"
r1.color = "red"
r1.weight = 30

Robot r2 = new Robot();
r2.name = "Jerry"
r2.color = "blue"
r2.weight = 40

r1.introduceSelf();
r2.introduceSelf();

Class for object :

class Robot {
String name;
String color;
int weight;
}

void introduceSelf() {
System.out.println(
"My name is " + this.name
)
}

you can use contructors to simplify the formation of objects
new Robot() === a constructor but it is a default that java has built in

    Robot(String n, String c, int w){
        this.name = n;
        this.color = c;
        this.weight = w;
    }

How to use the contructor, when you use your custom construcor the default stops working.

    Robot r1 = new Robot("Tom", "red", 30);
    Robot r2 = new Robot("Jerry", "blue", 40);
