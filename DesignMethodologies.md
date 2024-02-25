# Design Methodologies Lab

#### **<ins>Q1. What do we mean by coupling and cohesion when discussing structured design?<ins>**


In structured design coupling refers to the relationship complexity between software modules. High coupling means that two or more modules are tightly connected with one another and when implementing changes in one module the behaviour of another module could be affected. Whereas in low coupling modules are much more independent and when implementing changes to one module the behaviour of another module will have no to little impact.  

Cohesion refers to the complexity of elements that work in conjunction within a module/method to fulfil a single purpose. High cohesion means that elements within a module are tied closely together and focus on a single purpose. Whereas low cohesion means elements are loosely connected to one another allowing them to be used for multiple purposes. 


#### Q2. What is the difference between top-down and bottom-up design? Which best describes a function oriented design?

The design process of the Top-Down model starts from the system as a whole. The complete system then gets broken down into smaller approachable units which provide more details. This process is repeated until the very last specification has been identified completing the design of the system. In other words we break down the main problem into smaller problems and solve them individually. 

Whereas in the Bottom-Up model the design process involves defining different parts of a system which are then developed and linked together to create bigger components that will eventually make up the complete system. This approach is often used by OOP languages allowing developers to make decisions early on at lower levels which encourages reusability of components.     

The Top-Down model describes a function oriented design as the approach involves repeatedly decomposing the system design into smaller units which clearly define a specific functionality. 



#### Q3. In which design methodology would a class diagram be most useful?

Class diagrams are used to visually represent the structure of a system. They are extremely useful within the Bottom-Up model (OOP) as they allow one not only to visually comprehend the relationship between classes/objects but also help design the structure of a system. 



#### Q4. What are the four pillars of object oriented programming? Give a single-sentence description of each.

`Abstraction`: In abstraction we only provide the user with just about enough information to use a specific method/object and hide the irrelevant information on how something works. 

`Encapsulation`: In encapsulation objects and their variables are privatised and can be only accessed through dedicated getter and setter methods in order to enforce an extra layer of security that prevents users from having direct access to the properties of a certain object. 

`Inheritance`: Inheritance allows us to reduce code duplication and improve the maintainability of our code as child classes are able to inherit common properties and methods from a parent class without having to be specified again. 

`Polymorphism`: Polymorphism is quite similar to inheritance it enables a child class to share common properties and methods of a parent class while being able to define its own unique behaviours. 



#### Q5. What is the strategy pattern? How would its implementation differ between a functional and object oriented system?

The strategy pattern refers to a behavioural design patters which enables a system to dynamically change the behaviour of its objects. This is achieved by encapsulating range of behaviours (e.g. functionalities) from which an object can choose/switch from at runtime.  It is the process of decoupling behaviours from an object’s core which improves the overall flexibility and reusability of a system as behaviours can be simply added or modified with impacting an object’s core. 

In a functional system the strategy pattern can be implemented by simply representing behaviours as functions which are then passed as parameters to higher-order functions. 

Whereas in OOP the strategy pattern could be implemented by developing a range of behaviours that are represented in classes where each class defines a clear behaviour. Such behaviour classes usually implement an interface which allows other objects to inherit the behaviours from and dynamically utilise them based on their requirements. 

`Source`: https://www.freecodecamp.org/news/a-beginners-guide-to-the-strategy-design-pattern/  



#### Q6. Imagine your is creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following? Give some justification for your decision.

The design methodology I would suggest is the Object-oriented design. As mentioned earlier in OOP we are able to make decisions early on at lower levels which not only encourages reusability but also improves maintainability making it easier to add and modify elements to a system. We are also able to implement the stragety pattern by creating dedicated classes that define a set of behaviours which in this case could be various payment methods that are not tied to a specific object that might represent a particular sector or product. This would mean that a set of behaviours can be inherited by multiple objects that are then able to dynamically switch them based on their current requirements/specifications which in this case it could be a specific product or service.