For our final project for CS246 during the Fall 2022 term, a peer and I made a variation of Tetris called Biquadris. It was written in C++ and adhered to many OOP principles. We also implemented many design patterns, followed MVC architecture, adhered to RAII idiom, and ensured the project had low coupling and high cohesion.

Biquadris uses RAII via unique_ptr for automatic resource management (boards, blocks, displays), ensuring proper cleanup without manual memory management. Encapsulation isolates game logic: Board manages grid state, Player handles player-specific data, and Level abstracts block generation strategies. Inheritance and polymorphism enable interchangeable level implementations (Level0 through Level4) that override generateBlock() for different block generation algorithms. Design patterns organize the architecture: Observer decouples Board (Subject) from TextDisplay/GraphicsDisplay (Observers) for automatic UI updates; Factory Method (createLevel()) instantiates level objects without exposing concrete classes; and Decorator-like effects (blind mode, ghost mode) add visual behaviors dynamically without modifying base display classes. Each module has a single responsibility and interacts with other modules through basic calls to public methods. Due to Policy 71, the source code of this project is only available upon request.

Best,
Naunidh Singh


