# **`Design Pattern`**

## **Creational Patterns**

### 1. Factory

### 2. Abstract Factory

### 3. Singleton

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
