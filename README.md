# CryptoZombie-Solidity

# Chapter 3 - State Variables and Integers

State variables are permanently stored in contract storage. This means they're written to the Ethereum blockchain. Think of them like writing to a DB.


# Chapter 4 - Math Operations

- Addition: x + y
- Subtraction: x - y,
- Multiplication: x * y
- Division: x / y
- Modulus / remainder: x % y (for example, 13 % 5 is 3, because if you divide 5 into 13, 3 is the remainder)

# Chapter 5 - Structs

```
struct Person {
  uint age;
  string name;
}
```

# Chapter 6 - Arrays

When you want a collection of something, you can use an array. There are two types of arrays in Solidity: fixed arrays and dynamic arrays:

```
// Array with a fixed length of 2 elements:
uint[2] fixedArray;
// another fixed Array, can contain 5 strings:
string[5] stringArray;
// a dynamic Array - has no fixed size, can keep growing:
uint[] dynamicArray;
```

You can also create an array of structs.

```
Person[] people;
```

You can declare an array as public

```
Person[] public people;
```

# Chapter 7 - Function Declaration

```
function eatHamburgers(string memory _name, uint _amount) public {
}
```

# Chapter 8 - Working with Structs and Arrays

```
struct Zombie {
        string name;
        uint dna;
    }

     Zombie[] public zombies;

    function createZombie (string memory _name, uint _dna) public {
        zombies.push(Zombie(_name,_dna));
    }
```

# Chapter 9 - Private Functions

```
function _createZombie (string memory _name, uint _dna) private {
        zombies.push(Zombie(_name,_dna));
    }
```