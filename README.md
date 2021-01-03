# **`Design Pattern`**

## **Creational Patterns**

### 1. Factory

#### Creator

- The 'factory' object that creates new products
- Implements 'factoryMethod' which returns newly created products

#### AbstractProduct

- Declares an interface for products

#### ConcreteProduct

- The product being created
- All products support the same interface (properties and methods)

---

### 2. Abstract Factory

#### AbstractFactory

- Declares an interface for creating products

#### ConcreteFactory

- A factory object that 'manufactures' new products
- The create() method returns new products

#### Products

- The product instances being created by the Tfactory

#### AbstractProduct

- Declares an interface for the products that are being created

---

### 3. Singleton

#### Singleton

- Defines getInstance() which returns the unique instance.
- Responsible for creating and managing the instance object.

---

## **Structural Patterns**

### 1. Adapter

#### Client

- Calls into Adapter to request a service

#### Adapter

- Implements the interface that the client expects or knows

#### Adaptee

- The object being adapted
  has a different interface from what the client expects or knows

---

### 2. Decorator

#### Client

- Maintains a reference to the decorated

#### Component

- Object to which additional functionality is added

#### Decorator

- **Wraps around** component by maintaining a reference to it
  defines an interface that conforms to component's interface
  implements the additional functionality

---

## **Behavioral Patterns**

### 1. Chain Of Responsibility

#### Client

- Initiates the request to a chain of handler objects

#### Handler

- Defines an interface for handling the requests
- Implements the successor link (returning 'this')

---

### 2. Strategy

#### Context

- Maintains a reference to the current strategy object
- Supports interface to allow clients to request strategy calculations
- Allows clients to change trategy

#### Strategy

- Implements the algorithm using the Strategy interface

---

### 3. State

#### Context

- Exposes an interface that supports clients of the service
- Maintains a reference to a state object that defines the current state
- Allows State objects to change its current state to a different state

#### State

- Encapsulates the state values and associated behavior of the state
