For our final project for CS246 during the Fall 2022 term, a peer and I made a variation of Tetris called Biquadris. It was written in C++ and adhered to many OOP principles. We also implemented many design patterns, followed MVC architecture, adhered to RAII idiom, and ensured the project had low coupling and high cohesion.

In the end, the game had over 25 classes (each with their own .cc and .h file) and one Makefile. All fields were private to promote encapsulation and all super classes were abstract to promote polymorphism. Each module has a single responsibility and interacts with other modules through basic calls to public methods. Due to Policy 71, the source code of this project is only available upon request.

Below is the final UML diagram for our project:

