# Java Arrays Cheat Sheet:

**1. Declaration and Initialization:**
```java
// Declaration
dataType[] arrayName;

// Initialization
dataType[] arrayName = new dataType[size];

// Initialization with values (using int as an example)
int[] arrayName = {1, 2, 3, 4, 5};
```

**2. Accessing Elements:**
```java
// Reading an element by index
dataType element = arrayName[index];

// Modifying an element by index
arrayName[index] = newValue;
```

**3. Array Length:**
```java
// Getting length.  Keep in mind that arrays are indexed from 0 through .length-1
int length = arrayName.length;
```

**4. Iterating Through Array:**
```java
for (int i = 0; i < arrayName.length; i++) {
    // Access array elements using arrayName[i]
}
```

**5. Enhanced for-loop:**
```java
for (dataType element : arrayName) {
    // Access array elements directly using 'element'
    // You cannot modify the array in this type of for-loop
}
```

**6. Arrays of Objects:**
```java
// Declare and create an array of objects
ClassName[] objArray = new ClassName[size];
```

**7. Array Methods:**
```java
// Sorting array
Arrays.sort(arrayName);

// Searching array
int index = Arrays.binarySearch(arrayName, key);
```

**8. Array Copy:**
```java
// Copying array
dataType[] newArray = Arrays.copyOf(arrayName, newArraySize);
```

**9. Common Pitfalls:**
- Arrays have fixed size.
- Indexing starts from 0.
- Watch for ArrayIndexOutOfBoundsException.
