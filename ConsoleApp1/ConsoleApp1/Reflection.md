1. Why did you use inheritance?
		- I used inheritance because the Car, Boat, Airplane, and Helicopter classes have similar features as vehicles. By inheriting from the Vehicle abstract class, they can reuse shared functionality and follow a common structure.
		In this task, all transport classes are derived from Vehicle, which has the abstract Move() method. Each subclass has its own implementation of this method while remaining identifiable as a type of vehicle.
		Inheritance is suitable here because each transport has an IS-A relationship with the vehicle.

2.Why did you use interfaces?
		- I used interfaces to define what a vehicle is capable of doing. For example, IFlyable signifies the ability to fly, IDriveable, the ability to drive, 
    and ISailable, the ability to sail. Depending on its capabilities, a vehicle may include one or more interfaces.
    
3.Can Helicopter inherit from both Vehicle and Airplane? Why or why not?
		- No. In C#, a class may only inherit from one parent class. Helicopters cannot inherit from Airplanes because they already inherit from Vehicles. 
    A class can implement numerous interfaces, but it cannot inherit from other classes.
    
4.Why can Helicopter implement both IFlyable and IDriveable?
		-A helicopter can fulfill the requirements of both IFlyable and IDriveable since interfaces can be combined. In contrast to classes, a class can implement several interfaces.
    If the helicopter is engineered to have both flying and driving capabilities, then adopting both interfaces accurately represents its functionalities.
    
5.If a Submarine can both sail and dive, how would you design it?
		- I would create a Submarine class that inherits from Vehicle and implements both ISailable and IDiveable. This allows the submarine to follow the contracts for sailing and diving while still being treated as a type of vehicle.
		Its Move() method can be customized to describe its movement, such as "Diving underwater."

