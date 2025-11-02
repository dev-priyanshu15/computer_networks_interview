# Object-Oriented Programming (OOP) - Complete Notes with Code Examples

## What is Object-Oriented Programming?
OOP is a programming technique in which things work around objects. An object is an entity that has:

- **State or Property** (data members)
- **Behaviour** (member functions)

**Purpose:** To bring programs closer to the real world, which increases:
- Readability
- Manageability
- Extensibility

**Example:** In a game like Tekken, the hero "Paul" is an object with:
- **Properties:** name, health (70%), level ('A')
- **Behaviours:** attack, defence, dance

---

## Class and Object

### What is a Class?
A class is a user-defined data type - like how int, char, string are built-in data types, you can create your own custom data type.

```cpp
class Hero {
    // properties and behaviours
};
```

### What is an Object?
An object is an instance of a class. Just like:
- `int a;` creates an integer variable
- `string str;` creates a string variable
- `Hero ramesh;` creates a Hero type variable (object)

### Basic Class Creation
```cpp
class Hero {
    int health;
};

int main() {
    // Static allocation
    Hero a;
    
    // Dynamic allocation
    Hero *b = new Hero();
    delete b;  // Manual destructor call
    
    return 0;
}
```

---

## Important Points to Remember

### 1. Constructor Rules
- No return type
- Same name as class
- Called automatically during object creation
- Once you write your own constructor, default constructor is removed

### 2. Destructor Rules
- No return type, no parameters
- Same name as class with `~` prefix
- Called automatically for static allocation
- Must call manually with `delete` for dynamic allocation

### 3. Copy Constructor
- Must use pass by reference to avoid infinite loop
- Default copy constructor does shallow copy
- Custom copy constructor for deep copy

### 4. Static Members
- Belong to class, not object
- Can be accessed without creating object
- Static functions can only access static members
- No this keyword in static functions

### 5. Inheritance Access Table

| Base Class | Public Mode | Protected Mode | Private Mode |
|-----------|-------------|----------------|--------------|
| Public | Public | Protected | Private |
| Protected | Protected | Protected | Private |
| Private | Not Accessible | Not Accessible | Not Accessible |

### 6. Function Overloading Rules
- ✅ Different number of arguments
- ✅ Different types of arguments
- ❌ Only different return type (NOT allowed)

### 7. Operators that CANNOT be Overloaded
- `::`  (Scope resolution)
- `.*`  (Pointer to member)
- `.`   (Member access)
- `?:`  (Ternary operator)

---

## Homework Topics

### 1. Padding and Greedy Alignment
Study why size of object is 8 instead of 5 when it has int (4 bytes) + char (1 byte).

### 2. const Keyword
- How to use const with objects
- How to create const member functions

**Example:**
```cpp
class Hero {
public:
    int health;
    
    // const member function
    int getHealth() const {
        return health;
    }
};

int main() {
    const Hero h;
    // Can only call const member functions
    h.getHealth();
    return 0;
}
```

### 3. Initialization List
Alternative way to initialize data members in constructor.

**Example:**
```cpp
class Hero {
    int health;
    char level;
    
public:
    // Using initialization list
    Hero(int h, char l) : health(h), level(l) {
        cout << "Constructor called" << endl;
    }
};
```

### 4. Interface
Study about pure virtual functions and abstract classes.

### 5. Friend Function
Study how to use friend functions to access private members.

**Example:**
```cpp
class Hero {
private:
    int health;
    
public:
    friend void printHealth(Hero h);
};

void printHealth(Hero h) {
    cout << h.health << endl;  // Can access private member
}
```

---

## Benefits of OOP

### 1. Code Reusability
- Write once, use many times
- Inheritance allows reusing parent class code

### 2. Data Security
- Encapsulation hides data
- Only accessible through controlled methods

### 3. Easy to Maintain
- Changes in one class don't affect others
- Modular structure

### 4. Code Organization
- Better structure and readability
- Real-world modeling

### 5. Extensibility
- Easy to add new features
- Can extend existing classes

---

## Common Interview Questions

**Q1: What is OOP?**

Answer: Programming technique where things work around objects. An object has properties (state) and behaviors (functions).

**Q2: What is difference between class and object?**

Answer: Class is a user-defined data type (blueprint). Object is an instance of class (actual implementation).

**Q3: Why pass by reference in copy constructor?**

Answer: To avoid infinite loop. Pass by value would create copy, which calls copy constructor, which creates copy, leading to infinite recursion.

**Q4: What is shallow copy vs deep copy?**

Answer:
- **Shallow copy:** Copies pointer address, both objects point to same memory
- **Deep copy:** Creates new memory and copies values, separate memory for each object

**Q5: What are the four pillars of OOP?**

Answer:
1. **Encapsulation:** Wrapping data and functions together
2. **Inheritance:** Deriving properties from parent class
3. **Polymorphism:** Existing in multiple forms
4. **Abstraction:** Implementation hiding

**Q6: What is difference between encapsulation and abstraction?**

Answer:
- **Encapsulation:** Information hiding (data security)
- **Abstraction:** Implementation hiding (hiding complexity)

**Q7: What is difference between function overloading and function overriding?**

Answer:
- **Overloading:** Multiple functions with same name but different parameters (Compile time)
- **Overriding:** Child class redefines parent class function (Run time)

**Q8: When is destructor called automatically?**

Answer: For static allocation. For dynamic allocation, must call manually using `delete`.

**Q9: Can static function access non-static members?**

Answer: No. Static functions can only access static members. They have no this pointer.

**Q10: What is empty class size?**

Answer: 1 byte, for identification/tracking purposes.

---

## Practice Questions

### Exercise 1: Create a Student Class
Create a fully encapsulated Student class with:
- Private: name, rollNumber, marks
- Public: getters, setters, display function

### Exercise 2: Implement Inheritance
Create Animal → Dog → GermanShepherd hierarchy with appropriate functions.

### Exercise 3: Function Overloading
Create a Calculator class with multiple `add()` functions for different data types.

### Exercise 4: Operator Overloading
Overload `+` operator to add two Complex number objects.

### Exercise 5: Deep Copy
Create a class with dynamic memory allocation and implement deep copy constructor.

---

## Additional Resources

- **Code Studio:** Complete documentation available
- **Love Babbar OOPs Cheat Sheet:** Search "Love Babbar OOPs" on Google
- **Stack Overflow:** For encapsulation vs abstraction confusion

---

## Real World vs Academic OOP

**Important Note:**

The OOP we study here is basic level for interviews and understanding fundamentals.

**In real industry:**
- OOP is used extensively for code reusability and maintainability
- More focused on design patterns
- Machine coding rounds (like in Flipkart) test advanced OOP

**Future Course:** A dedicated OOP course will cover:
- Advanced design patterns
- Machine coding round preparation
- Industry-level OOP applications
- Real-world project structures

---

## Final Summary

### What We Learned:

**Basic Concepts:**
1. Class and Object creation
2. Access Modifiers (public, private, protected)
3. Getters and Setters
4. Static vs Dynamic Allocation
5. Size of objects and padding

**Advanced Concepts:**
6. Constructors (Default, Parameterized, Copy)
7. this keyword
8. Destructor
9. Shallow vs Deep Copy
10. Copy Assignment Operator
11. Static members and functions

**Four Pillars:**
12. **Encapsulation:** Data + Functions together
13. **Inheritance:** 5 types, 3 modes, ambiguity resolution
14. **Polymorphism:** Compile time (overloading) + Run time (overriding)
15. **Abstraction:** Implementation hiding

---

## Key Code Examples Summary

```cpp
// 1. Basic Class
class Hero {
    int health;
public:
    char level;
};

// 2. Constructor
Hero(int h) : health(h) {}

// 3. Copy Constructor
Hero(Hero &temp) {
    this->health = temp.health;
}

// 4. Destructor
~Hero() {
    cout << "Destructor called" << endl;
}

// 5. Static Member
static int timeToComplete;
int Hero::timeToComplete = 5;

// 6. Inheritance
class Dog : public Animal {
};

// 7. Function Overloading
void display(int x) {}
void display(string x) {}

// 8. Operator Overloading
void operator+ (B &obj) {
    cout << "Overloaded" << endl;
}

// 9. Function Overriding
class Dog : public Animal {
    void speak() {  // Overrides Animal's speak()
        cout << "Barking" << endl;
    }
};

// 10. Scope Resolution (Ambiguity)
obj.A::func();  // Calls A's function
obj.B::func();  // Calls B's function
```

---

**Remember:** Practice is key! Implement all examples yourself and try creating your own classes. Good luck with your OOP journey! 🚀

That's it for this comprehensive OOP guide. We will meet in the next topic. Bye bye!Hero h1;
    cout << "size: " << sizeof(h1) << endl;  // Output: 4 (size of int)
    return 0;
}
```

### Empty Class Size
```cpp
class Hero {
    // empty class
};

int main() {
    Hero h1;
    cout << sizeof(h1) << endl;  // Output: 1
    return 0;
}
```

**Important:** Empty class gives 1 byte for identification/tracking purposes.

---

## Access Modifiers

There are 3 types of access modifiers that control where data members can be accessed:

1. **Public:** Can be accessed inside and outside the class
2. **Private:** Can be accessed inside the class only
3. **Protected:** Can be accessed inside the class and by derived/child classes

**Default access modifier in class is PRIVATE.**

```cpp
class Hero {
private:
    int health;      // private by default
    
public:
    char level;      // public - accessible everywhere
    
    void print() {
        cout << level << endl;  // can access private 'health' here
    }
};

int main() {
    Hero ramesh;
    ramesh.level = 'A';    // OK - public member
    // ramesh.health = 70;  // ERROR - private member
    return 0;
}
```

---

## Getters and Setters

When data members are private, we use getter and setter functions to access them.

```cpp
class Hero {
private:
    int health;
    char level;
    
public:
    // Getter functions
    int gethealth() {
        return health;
    }
    
    char getlevel() {
        return level;
    }
    
    // Setter functions
    void sethealth(int h) {
        health = h;
    }
    
    void setlevel(char ch) {
        level = ch;
    }
};

int main() {
    Hero ramesh;
    ramesh.sethealth(70);
    ramesh.setlevel('A');
    
    cout << "Ramesh health is " << ramesh.gethealth() << endl;  // Output: 70
    return 0;
}
```

**Benefits of Setter:**
- Can add validation conditions
- Can add password protection
- Can restrict who can modify the data

```cpp
void sethealth(int h, char name) {
    if(name == 'A') {  // only user 'A' can change health
        health = h;
    }
}
```

---

## Static vs Dynamic Allocation

### Static Allocation
```cpp
Hero a;  // created on stack
cout << "level is " << a.level << endl;
cout << "health is " << a.gethealth() << endl;
```

### Dynamic Allocation
```cpp
Hero *b = new Hero;  // created on heap

// Two ways to access:
// Method 1: Dereference first
cout << (*b).gethealth() << endl;

// Method 2: Arrow operator (better way)
cout << b->gethealth() << endl;

b->sethealth(70);
b->setlevel('A');
```

---

## Constructors

A constructor:
- Is invoked during object creation time
- Has no return type
- Has the same name as class

### 1. Default Constructor
```cpp
class Hero {
public:
    Hero() {
        cout << "Constructor called" << endl;
    }
};

int main() {
    cout << "Hi" << endl;
    Hero ramesh;    // Constructor called here
    cout << "Hello" << endl;
    
    // Output:
    // Hi
    // Constructor called
    // Hello
    
    return 0;
}
```

**Note:** Once you write your own constructor, the inbuilt default constructor will be removed.

### 2. Parameterized Constructor
```cpp
class Hero {
private:
    int health;
    char level;
    
public:
    // Parameterized constructor
    Hero(int health) {
        this->health = health;
    }
    
    Hero(int health, char level) {
        this->health = health;
        this->level = level;
    }
};

int main() {
    Hero ramesh(10);           // calls first constructor
    Hero temp(22, 'B');        // calls second constructor
    
    // Dynamic allocation
    Hero *h = new Hero(11);
    
    return 0;
}
```

---

## The "this" Keyword

`this` is a pointer that stores the address of the current object.

```cpp
class Hero {
    int health;
    
public:
    Hero(int health) {
        this->health = health;  // this->health refers to object's health
                                // health refers to parameter
    }
};

int main() {
    Hero ramesh(10);
    cout << &ramesh << endl;     // prints address of ramesh
    // Inside constructor, 'this' contains the same address
    
    return 0;
}
```

**Use:** When parameter name and data member name are same, this helps distinguish between them.

---

## Copy Constructor

A copy constructor creates a new object as a copy of an existing object.

```cpp
class Hero {
private:
    int health;
    char level;
    
public:
    Hero() {}
    
    Hero(int health, char level) {
        this->health = health;
        this->level = level;
    }
    
    // Copy constructor (must use pass by reference)
    Hero(Hero &temp) {
        cout << "Copy constructor called" << endl;
        this->health = temp.health;
        this->level = temp.level;
    }
    
    void print() {
        cout << "Health: " << this->health << endl;
        cout << "Level: " << this->level << endl;
    }
};

int main() {
    Hero S(70, 'C');
    S.print();
    
    // Two ways to call copy constructor:
    Hero R(S);        // Method 1
    Hero R = S;       // Method 2 (same as above)
    
    R.print();  // Same values as S
    
    return 0;
}
```

**Important:** Copy constructor must use pass by reference (Hero &temp).

### Why Pass by Reference?
- If you use pass by value, it creates a copy
- To create that copy, copy constructor is called
- This calls copy constructor again → infinite loop
- Pass by reference avoids creating a copy

---

## Shallow Copy vs Deep Copy

### Shallow Copy (Default Copy Constructor)

```cpp
class Hero {
public:
    char *name;
    int health;
    char level;
    
    Hero() {
        name = new char[100];
    }
    
    void setname(char name[]) {
        strcpy(this->name, name);
    }
    
    void print() {
        cout << "Name: " << this->name << endl;
        cout << "Health: " << this->health << endl;
        cout << "Level: " << this->level << endl;
    }
};

int main() {
    Hero hero1;
    char name[7] = "Babbar";
    hero1.setname(name);
    hero1.sethealth(12);
    hero1.setlevel('D');
    hero1.print();  // Output: Babbar, 12, D
    
    // Using default copy constructor (shallow copy)
    Hero hero2(hero1);
    hero2.print();  // Output: Babbar, 12, D
    
    hero1.name[0] = 'G';
    hero1.print();  // Output: Gabbar, 12, D
    hero2.print();  // Output: Gabbar, 12, D (also changed!)
    
    return 0;
}
```

**Problem:** In shallow copy, both objects point to the same memory location. Changing one affects the other.

### Deep Copy (Custom Copy Constructor)

```cpp
class Hero {
public:
    char *name;
    int health;
    char level;
    
    Hero() {
        name = new char[100];
    }
    
    // Deep copy constructor
    Hero(Hero &temp) {
        char *ch = new char[strlen(temp.name) + 1];
        strcpy(ch, temp.name);
        this->name = ch;
        
        this->health = temp.health;
        this->level = temp.level;
    }
    
    void setname(char name[]) {
        strcpy(this->name, name);
    }
    
    void print() {
        cout << "Name: " << this->name << endl;
        cout << "Health: " << this->health << endl;
        cout << "Level: " << this->level << endl;
    }
};

int main() {
    Hero hero1;
    char name[7] = "Babbar";
    hero1.setname(name);
    hero1.print();  // Output: Babbar
    
    // Using deep copy constructor
    Hero hero2(hero1);
    hero2.print();  // Output: Babbar
    
    hero1.name[0] = 'G';
    hero1.print();  // Output: Gabbar
    hero2.print();  // Output: Babbar (unchanged!)
    
    return 0;
}
```

**Solution:** In deep copy, a new array is created with separate memory location.

---

## Copy Assignment Operator

When objects are already created and you want to copy one to another, use copy assignment operator `=`.

```cpp
int main() {
    Hero hero1;
    char name[7] = "Gabbar";
    hero1.setname(name);
    
    Hero hero2;
    char name2[7] = "Babbar";
    hero2.setname(name2);
    
    hero1.print();  // Output: Gabbar
    hero2.print();  // Output: Babbar
    
    // Copy assignment
    hero1 = hero2;
    
    hero1.print();  // Output: Babbar
    hero2.print();  // Output: Babbar
    
    return 0;
}
```

**Difference from Copy Constructor:**
- **Copy Constructor:** Creates new object while copying
- **Copy Assignment:** Both objects already exist, then copy

---

## Destructor

A destructor:
- Deallocates memory
- Is called when object goes out of scope
- Has same name as class with `~` prefix
- Has no return type
- Has no parameters

```cpp
class Hero {
public:
    Hero() {
        cout << "Simple constructor called" << endl;
    }
    
    ~Hero() {
        cout << "Destructor bhai called" << endl;
    }
};

int main() {
    Hero a;              // Static allocation
    Hero *b = new Hero;  // Dynamic allocation
    
    delete b;  // Manual destructor call for dynamic allocation
    
    // For static object 'a', destructor called automatically
    
    return 0;
}
```

**Important:**
- **Static allocation:** Destructor called automatically
- **Dynamic allocation:** Must call destructor manually using `delete`

---

## Static Keyword

### Static Data Members

Static data members belong to the class, not to any object. Can be accessed without creating an object.

```cpp
class Hero {
public:
    int health;
    char level;
    static int timeToComplete;  // static member
};

// Initialize static member outside class
int Hero::timeToComplete = 5;

int main() {
    // Access without creating object
    cout << Hero::timeToComplete << endl;  // Output: 5
    
    Hero a;
    cout << a.timeToComplete << endl;  // Output: 5 (not recommended)
    
    Hero b;
    b.timeToComplete = 10;
    
    cout << Hero::timeToComplete << endl;  // Output: 10
    cout << a.timeToComplete << endl;      // Output: 10
    
    return 0;
}
```

### Static Member Functions

```cpp
class Hero {
public:
    int health;
    static int timeToComplete;
    
    static int random() {
        // Can only access static members
        return timeToComplete;
    }
};

int Hero::timeToComplete = 5;

int main() {
    cout << Hero::random() << endl;  // Access without object
    return 0;
}
```

**Properties of Static Functions:**
- No need to create object to call them
- Call using class name
- No this keyword (because no object)
- Can only access static members

---

## Size and Padding

```cpp
class Hero {
    int health;   // 4 bytes
    char level;   // 1 byte
};

int main() {
    Hero ramesh;
    cout << "Size of Ramesh is " << sizeof(ramesh) << endl;
    // Expected: 4 + 1 = 5
    // Actual Output: 8
    
    return 0;
}
```

**Why 8 instead of 5?** Due to padding and greedy alignment (Homework topic).

---

## Four Pillars of OOP

## 1. Encapsulation

**Definition:** Wrapping up data members and functions into a single entity (class).

Think of it like a capsule:
- Red spheres = data members
- White spheres = functions
- Capsule = class

When you wrap data members and functions in a class, you achieve encapsulation.

```cpp
class Student {
private:
    string name;
    int age;
    int height;

public:
    int getAge() {
        return this->age;
    }
};

int main() {
    Student first;
    cout << "Sab sahi chalra hai" << endl;
    return 0;
}
```

### Fully Encapsulated Class

A class where all data members are marked private.

```cpp
class Hero {
private:
    int health;
    char level;
    string name;
    
public:
    int getHealth() { return health; }
    void setHealth(int h) { health = h; }
    
    char getLevel() { return level; }
    void setLevel(char l) { level = l; }
};
```

### Advantages of Encapsulation

1. **Data Hiding (Information Hiding)**
   - If marked private, no other class can access it directly
   - Can only access through getter/setter

2. **Increased Security**
   - Control who can read/write data

3. **Make Class Read-Only**
   - Provide getter but no setter
   - Data can be read but not modified

4. **Code Reusability**
   - Reuse the same class in different programs

5. **Unit Testing**
   - Easy to test individual classes

**Note:** Encapsulation = Information Hiding (Different from Abstraction which is Implementation Hiding)

---

## 2. Inheritance

**Definition:** The capability of a class to derive properties and characteristics from another class.

**Real Life Example:**
- Your height is same as your father (you inherited it)
- Your hair is silky like your mom's (you inherited it)

### Terminology
- **Parent Class / Super Class / Base Class:** The class being inherited from
- **Child Class / Sub Class / Derived Class:** The class that inherits

### Basic Inheritance Syntax

```cpp
class Human {
public:
    int height;
    int weight;
    int age;
    
    int getAge() {
        return age;
    }
    
    void setWeight(int w) {
        weight = w;
    }
};

class Male : public Human {
public:
    string color;
    
    void sleep() {
        cout << "Male Sleeping" << endl;
    }
};

int main() {
    Male object1;
    
    // Can access Human's properties through Male object
    cout << object1.age << endl;
    cout << object1.weight << endl;
    cout << object1.height << endl;
    cout << object1.color << endl;
    
    object1.setWeight(84);
    object1.sleep();
    
    return 0;
}
```

**Syntax:** `class ChildClass : access_modifier ParentClass`

### Modes of Inheritance

There are 3 modes: public, protected, private

**Inheritance Table:**

| Base Class Access | Public Mode | Protected Mode | Private Mode |
|------------------|-------------|----------------|--------------|
| Public | Public | Protected | Private |
| Protected | Protected | Protected | Private |
| Private | Not Accessible | Not Accessible | Not Accessible |

**Important:** Private members of parent class cannot be inherited in any mode.

### Protected Access Modifier

Protected works similar to private with one difference:
- **Private:** Accessible only inside the class
- **Protected:** Accessible inside the class + accessible in derived/child classes

```cpp
class Human {
protected:
    int height;  // protected member
};

class Male : public Human {
public:
    int getHeight() {
        return this->height;  // Can access protected member
    }
};

int main() {
    Male m1;
    // m1.height;  // ERROR - can't access outside
    cout << m1.getHeight() << endl;  // OK - access through function
    return 0;
}
```

---

## Types of Inheritance

### 1. Single Inheritance

One class inherits from one parent class.

```cpp
class Animal {
public:
    int age;
    int weight;
    
    void speak() {
        cout << "Speaking" << endl;
    }
};

class Dog : public Animal {
};

int main() {
    Dog d;
    d.speak();
    cout << d.age << endl;
    return 0;
}
```

**Structure:** A → B

### 2. Multi-Level Inheritance

Inheritance at multiple levels (chain of inheritance).

```cpp
class Animal {
public:
    int age;
    int weight;
    
    void speak() {
        cout << "Speaking" << endl;
    }
};

class Dog : public Animal {
};

class GermanShepherd : public Dog {
};

int main() {
    GermanShepherd g;
    g.speak();  // Can access Animal's function
    return 0;
}
```

**Structure:** A → B → C

### 3. Multiple Inheritance

One class inherits from more than one parent class.

```cpp
class Animal {
public:
    void bark() {
        cout << "Barking" << endl;
    }
};

class Human {
public:
    string color;
    
    void speak() {
        cout << "Speaking" << endl;
    }
};

// Multiple Inheritance
class Hybrid : public Animal, public Human {
};

int main() {
    Hybrid obj1;
    obj1.speak();  // From Human
    obj1.bark();   // From Animal
    return 0;
}
```

**Structure:** A, B → C

**Syntax:** `class C : public A, public B`

### 4. Hierarchical Inheritance

One parent class serves as base class for multiple child classes.

```cpp
class A {
public:
    void func1() {
        cout << "Inside Function 1" << endl;
    }
};

class B : public A {
public:
    void func2() {
        cout << "Inside Function 2" << endl;
    }
};

class C : public A {
public:
    void func3() {
        cout << "Inside Function 3" << endl;
    }
};

int main() {
    A object1;
    object1.func1();
    
    B object2;
    object2.func1();  // From A
    object2.func2();  // From B
    
    C object3;
    object3.func1();  // From A
    object3.func3();  // From C
    
    return 0;
}
```

**Structure:**
```
      A
     / \
    B   C
```

### 5. Hybrid Inheritance

Combination of more than one type of inheritance.

```cpp
// Example: Combination of Hierarchical + Multiple
class A {
public:
    void func1() {
        cout << "Inside A" << endl;
    }
};

class B : public A {
public:
    void func2() {
        cout << "Inside B" << endl;
    }
};

class D {
public:
    void func4() {
        cout << "Inside D" << endl;
    }
};

// C inherits from both A and D (Multiple Inheritance)
class C : public A, public D {
public:
    void func3() {
        cout << "Inside C" << endl;
    }
};
```

**Structure:** Mix of multiple inheritance types

---

## Inheritance Ambiguity

**Problem:** When two parent classes have functions with the same name, which one gets called?

```cpp
class A {
public:
    void func() {
        cout << "I am A" << endl;
    }
};

class B {
public:
    void func() {
        cout << "I am B" << endl;
    }
};

class C : public A, public B {
};

int main() {
    C obj;
    // obj.func();  // ERROR - Ambiguous! Which func()?
    
    // Solution: Use scope resolution operator
    obj.A::func();  // Calls A's func()
    obj.B::func();  // Calls B's func()
    
    return 0;
}
```

**Solution:** Use scope resolution operator `::` to specify which class's function to call.

---

## 3. Polymorphism

**Definition:** Poly = Many, Morph = Forms → Existing in multiple forms.

**Real Life Example:**
- Your father is a son (to his mother)
- Your father is a husband (to your mother)
- Your father is a father (to you)
- Your father is a brother (to your aunt)

Same person, multiple forms!

### Types of Polymorphism

1. **Compile Time Polymorphism** (Static Polymorphism)
2. **Run Time Polymorphism** (Dynamic Polymorphism)

---

## A. Compile Time Polymorphism

We know at compile time which form will be used.

### 1. Function Overloading

Having multiple functions with the same name but different parameters.

```cpp
class A {
public:
    void sayHello() {
        cout << "Hello Love Babbar" << endl;
    }
    
    void sayHello(string name) {
        cout << "Hello " << name << endl;
    }
    
    int sayHello(char name) {
        cout << "Hello Love Babbar" << endl;
        return 1;
    }
};

int main() {
    A obj;
    obj.sayHello();           // Calls 1st function
    obj.sayHello("Ramesh");   // Calls 2nd function
    obj.sayHello('R');        // Calls 3rd function
    return 0;
}
```

**Rules for Function Overloading:**
- Different number of arguments, OR
- Different types of arguments
- Cannot overload by changing only return type

**Examples:**

```cpp
// Different number of arguments
int add(int a, int b) { return a + b; }
int add(int a, int b, int c) { return a + b + c; }

// Different types of arguments
void display(int x) { cout << x; }
void display(double x) { cout << x; }
void display(string x) { cout << x; }
void display(char x) { cout << x; }

// Default arguments
int add(int x, int y, int z = 0, int w = 0) {
    return x + y + z + w;
}
// Can call: add(1, 2) OR add(1, 2, 3) OR add(1, 2, 3, 4)
```

### 2. Operator Overloading

Giving new meaning to existing operators.

**Operators that CAN be overloaded:** `+`, `-`, `*`, `/`, `%`, `++`, `--`, `==`, `!=`, `<`, `>`, `<=`, `>=`, `&&`, `||`, `!`, `&`, `|`, `^`, `~`, `<<`, `>>`, `=`, `+=`, `-=`, `*=`, `/=`, `%=`, `[]`, `()`, `->`, `new`, `delete`

**Operators that CANNOT be overloaded:** `::`, `.*`, `.`, `?:`

```cpp
class B {
public:
    int a;
    int b;
    
    // Overloading '+' operator to do subtraction
    void operator+ (B &obj) {
        int value1 = this->a;
        int value2 = obj.a;
        cout << "output " << value2 - value1 << endl;
    }
    
    // Overloading '()' operator
    void operator() () {
        cout << "main Bracket hu " << this->a << endl;
    }
};

int main() {
    B obj1, obj2;
    
    obj1.a = 4;
    obj2.a = 7;
    
    obj1 + obj2;  // Calls operator+ function, Output: 3
    obj1();       // Calls operator() function
    
    return 0;
}
```

**Another Example:**

```cpp
class B {
public:
    int a;
    int b;
    
    void operator+ (B &obj) {
        cout << "Hello Babbar" << endl;
    }
};

int main() {
    B obj1, obj2;
    obj1 + obj2;  // Prints: Hello Babbar
    return 0;
}
```

---

## B. Run Time Polymorphism

We know at run time which form is being used.

### Method Overriding (Function Overriding)

Child class provides its own implementation of a function that is already defined in parent class.

```cpp
class Animal {
public:
    void speak() {
        cout << "Speaking" << endl;
    }
};

class Dog : public Animal {
public:
    // Overriding parent's speak() function
    void speak() {
        cout << "Barking" << endl;
    }
};

int main() {
    Dog obj;
    obj.speak();  // Output: Barking (calls Dog's speak)
    return 0;
}
```

**Rules for Method Overriding:**
- Method in parent and child class must have same name
- Must have same parameters
- Only possible through inheritance

**Use Case:**
- Parent class has 10 methods
- Child class wants to use 8 methods as-is
- Child class wants to implement 2 methods in its own way
- This is code reusability + custom implementation

**Example:**

```cpp
class Animal {
public:
    void speak() {
        cout << "Speaking" << endl;
    }
};

class Dog : public Animal {
    // If you don't override, parent's speak() will be called
    // If you override, your own speak() will be called
};

int main() {
    Dog obj;
    obj.speak();  // If no override: "Speaking"
                  // If override exists: "Barking"
    return 0;
}
```

---

## 4. Abstraction

**Definition:** Implementation Hiding - showing only essential information and hiding details.

**Synonym:** Implementation Hiding

**Real Life Example:**
- When you send an email, you just click "Send"
- You don't need to know which protocol is being used (SMTP)
- You don't need to know the design patterns
- You only see what's necessary

### How to Achieve Abstraction

Use access modifiers to control what is visible and what is hidden.

```cpp
class Hero {
private:
    int health;      // Hidden from outside
    string name;     // Hidden from outside
    
public:
    void setHealth(int h) {   // Visible to outside
        health = h;
    }
    
    int getHealth() {          // Visible to outside
        return health;
    }
};
```

### Advantages of Abstraction

1. **Data hiding / Security**
   - Only essential information is exposed

2. **Code reusability**
   - Can change internal implementation without affecting users

3. **Avoids code duplication**
   - Common functionality in one place

4. **Easy to maintain**
   - Changes in implementation don't affect users

---

## Encapsulation vs Abstraction

Many students get confused between these two!

| Encapsulation | Abstraction |
|--------------|-------------|
| Wrapping data and functions together | Showing only essential features |
| Information Hiding | Implementation Hiding |
| About data security | About hiding complexity |
| Achieved by making data members private and providing getters/setters | Achieved by using access modifiers and interfaces |

---

## Summary - Four Pillars of OOP

### 1. Encapsulation
- Wrapping data members and functions in a class
- Fully encapsulated = all data members private
- Benefits: Data hiding, security, read-only classes, code reusability

### 2. Inheritance
- Deriving properties from parent class to child class
- 5 Types: Single, Multi-level, Multiple, Hierarchical, Hybrid
- 3 Modes: public, protected, private
- Use `::` for inheritance ambiguity

### 3. Polymorphism
- Existing in multiple forms
- Compile Time: Function Overloading, Operator Overloading
- Run Time: Method Overriding

### 4. Abstraction
- Implementation hiding
- Show only essential information
- Use access modifiers to achieve it

---

## Complete Hero Class Example

```cpp
#include<iostream>
using namespace std;

class Hero {
private:
    int health;

public:
    char *name;
    char level;
    static int timeToComplete;

    Hero() {
        cout << "Simple constructor called" << endl;
        name = new char[100];
    }

    Hero(int health) {
        this->health = health;
    }

    Hero(int health, char level) {
        this->level = level;
        this->health = health;
    }

    // Copy constructor
    Hero(Hero& temp) {
        char *ch = new char[strlen(temp.name) + 1];
        strcpy(ch, temp.name);
        this->name = ch;

        cout << "Copy constructor called" << endl;
        this->health = temp.health;
        this->level = temp.level;
    }

    void print() {
        cout << endl;
        cout << "[ Name: " << this->name << " ,";
        cout << "health: " << this->health << " ,";
        cout << "level: " << this->level << " ]";
        cout << endl << endl;
    }

    int getHealth() {
        return health;
    }

    char getLevel() {
        return level;
    }

    void setHealth(int h) {
        health = h;
    }

    void setLevel(char ch) {
        level = ch;
    }

    void setName(char name[]) {
        strcpy(this->name, name);
    }

    static int random() {
        return timeToComplete;
    }

    // Destructor
    ~Hero() {
        cout << "Destructor bhai called" << endl;
    }
};

int Hero::timeToComplete = 5;

int main() {
