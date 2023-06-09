# Objects:
## At the end of the session , you will be able to :

- Define what an object is and how it is used in JavaScript.
- Perform common operations on objects, including inserting new properties, reading property values, updating property values, and deleting properties.
- Create a simple nested object by defining an object within an object.
- Create a complex nested object by defining multiple objects within an object and including arrays as properties.


## Object: 

- In programming, an object is a collection of properties that represent a real-world entity or concept. It is a data structure that groups related data and functions into a single unit. Objects are used to model complex systems and can be used to represent anything from a person to a car to a company. In JavaScript, objects are created using curly braces {} and consist of key-value pairs.

### Operations on Objects:

- Insertion: You can add a new property to an object by using the dot notation or square brackets.
  Here's an example:

```js
const person = {
  name: "Geekster",
  age: 25,
};

person.email = "john@example.com"; // dot notation
person["phone"] = "1234567890"; // square brackets
```

## Reading:

- You can access the value of a property in an object using the dot notation or square brackets. Here's an example:

```js
const person = {
  name: "John",
  age: 25,
  email: "john@example.com",
  phone: "1234567890",
};

console.log(person.name); // Output: "John"
console.log(person["age"]); // Output: 25
```

## Updation:

- You can update the value of a property in an object using the dot notation or square brackets.
  Here's an example:

```js
const person = {
  name: "John",
  age: 25,
  email: "john@example.com",
  phone: "1234567890",
};

person.age = 26; // dot notation
person["phone"] = "0987654321"; // square brackets
```

## Deletion:

- You can remove a property from an object using the delete keyword. Here's an example:

```js
const person = {
  name: "John",
  age: 25,
  email: "john@example.com",
  phone: "1234567890",
};

delete person.email;
```

## Creating a Simple Nested Object:

A nested object is an object that contains one or more properties that are also objects.
Here's an example of a simple nested object:

```js
const person = {
  name: "John",
  age: 25,
  contact: {
    email: "john@example.com",
    phone: "1234567890",
  },
};
```

## JSON:

JSON (JavaScript Object Notation) is a lightweight data interchange format that is easy for humans to read and write, and easy for machines to parse and generate. It is a text format that is completely language-independent but uses conventions that are familiar to programmers of the C family of languages, including C, C++, C#, Java, JavaScript, Perl, Python, and many others. JSON is used to transmit data between a server and a web application, as an alternative to XML.

## Creating a Complex Nested Object:

A complex nested object is an object that contains multiple levels of nesting. Here's an example:

```js
const company = {
  name: "ABC Corp",
  employees: [
    {
      name: "John",
      age: 25,
      contact: {
        email: "john@example.com",
        phone: "1234567890",
      },
    },
    {
      name: "Mary",
      age: 30,
      contact: {
        email: "mary@example.com",
        phone: "0987654321",
      },
    },
  ],
  location: {
    address: "123 Main St",
    city: "Anytown",
    state: "CA",
    zip: "12345",
  },
};
```

# Further reading :

### Object Methods

There are different methods to manipulate an object. Let us see some of the available methods.

_Object.assign_: To copy an object without modifying the original object

```js
const person = {
  firstName: "Asabeneh",
  age: 250,
  country: "Finland",
  city: "Helsinki",
  skills: ["HTML", "CSS", "JS"],
  title: "teacher",
  address: {
    street: "Heitamienkatu 16",
    pobox: 2002,
    city: "Helsinki",
  },
  getPersonInfo: function () {
    return `I am ${this.firstName} and I live in ${this.city}, ${this.country}. I am ${this.age}.`;
  },
};

//Object methods: Object.assign, Object.keys, Object.values, Object.entries
//hasOwnProperty

const copyPerson = Object.assign({}, person);
console.log(copyPerson);
```

#### Getting object keys using Object.keys()

_Object.keys_: To get the keys or properties of an object as an array

```js
const keys = Object.keys(copyPerson);
console.log(keys); //['firstName', 'age', 'country','city', 'skills','title', 'address', 'getPersonInfo']
const address = Object.keys(copyPerson.address);
console.log(address); //['street', 'pobox', 'city']
```

#### Getting object values using Object.values()

_Object.values_:To get values of an object as an array

```js
const values = Object.values(copyPerson);
console.log(values);
```

#### Getting object keys and values using Object.entries()

_Object.entries_:To get the keys and values in an array

```js
const entries = Object.entries(copyPerson);
console.log(entries);
```

#### Checking properties using hasOwnProperty()

_hasOwnProperty_: To check if a specific key or property exist in an object

```js
console.log(copyPerson.hasOwnProperty("name"));
console.log(copyPerson.hasOwnProperty("score"));
```
