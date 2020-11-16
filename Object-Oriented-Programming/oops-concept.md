What is OOPS and Why We Need OOPS.

What is OOPS:
            Object-oriented programming (OOP) is a programming paradigm based on the concept of "objects", which can contain data and code: data in the form of fields (often known as attributes or properties), and code, in the form of procedures (often known as methods). (Wiki)

            Before oops we have "Procedural Programming"  
            Procedural Programming: Divided a program into set of functions.
                                    so we have data stored in a bunch of variables
                                    and functions that operate on the data.

                                    Adavantages : very simple and straightforward.
                                    Disadvantage : As program grow it will end up with a
                                                   bunch of functions that are all over the place you need to copy and pasting the func over and over.
                                                   if you change one func other serveral functions break.
                                                   so much interdependance between all these functions.

           Object-Oriented Programming Solve this Problem.  
                In OOPS we combine  a group of related variables and functions into 
                a unit and we call that unit object.
                we refer to these varibles as properties.
                and the functions as methods.

            1. Encapsulation : we group related variables and functions that operate on
                               them into objects and this is we called encapsulation.
                               Reduce complexity + increase reusability

                               Example:

                               // Procedural way

                               var baseSalary int = 2500;
                               var overtime int = 10;
                               var rate int 20;

                               func getWage(baseSalary,overtime,rate){ // there params
                                return baseSalary + (overtime * rate);
                               }

                               // Object Orienred way

                               var employee = {
                                   baseSalary int = 2500,
                                   overtime int = 10,
                                   rate int 20,

                                   getWage: function(){ // no params
                                       return this.baserSalary+(this.overtime * this.rate);
                                   }
                               };

                               employee.getWage(); 

                            


            2. Abstraction :    
                            "shows" only essential attributes and "hides" unnecessary     information.
                            Its main goal is to handle complexity by hiding unnecessary 
                            details from the user. 
                            For example, when you login to your bank account online, you enter your user_id and password and press login, what happens when you press login, how the input data sent to server, how it gets verified is all abstracted away from the you.
                            Advantage:
                            Reduce complexity + isolate impact of changes

                        

            3. Inheritance : 
                            The process by which one class acquires the properties and functionalities of another class is called inheritance.
                            Helps reduce redadent code.

            4. Polymorphism : 
                            Polymorphism is a object oriented programming feature that allows us to perform a single action in different ways. 
                            refactor ugly switch/case statements


            





                                   
