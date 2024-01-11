# Java Classes Cheat Sheet:

**1. Class Declaration:**
```java
public class ClassName {
    // Class members (fields, methods)
}
```

**2. Instance Variables:**
```java
private dataType variableName;  // Encapsulation with private access
```

**3. Constructors:**
```java
// Default Constructor
public ClassName() {
    // Initialize instance variables here
}

// Parameterized Constructor
public ClassName(dataType parameter1, dataType parameter2) {
    // Initialize instance using the values of the parameters
}
```

**4. Accessors (Getter Methods):**
```java
public dataType getVariableName() {
    return variableName;
}
```

**5. Mutators (Setter Methods):**
```java
public void setVariableName(dataType newValue) {
    this.fieldName = newValue;  // Using "this" to distinguish instance variable from parameter
}
```

**6. Equals Method (Override for Custom Comparisons):** 
```java
@Override
public boolean equals(Object obj) {
    if (this == obj) return true;  // Same reference
    if (obj == null || getClass() != obj.getClass())
        return false;  // Different types
    ClassName other = (ClassName) obj;
    return this.fieldName.equals(other.fieldName);  // Custom comparison
}
```

**7. toString Method (Override for String Representation):** 
```java
@Override public String toString() {
    return "ClassName{" +
            "variableName=" + variableName +
            '}';
}
```

**8. "this" Keyword:**
- Used to refer to the current instance of the class.
- Helps distinguish between instance variables and method parameters.
- Example: `this.variableName = parameter;`

**9. Example Usage:**
```java
ClassName obj1 = new ClassName();            // Creating an object using default constructor
obj1.setVariableName(value);                 // Using mutator to set field value
dataType value = obj1.getVariableName();     // Using accessor to retrieve field value
boolean isEqual = obj1.equals(otherObject);  // Using equals for custom comparison
String strRepresentation = obj1.toString();  // Using toString for string representation
```

**Remember:** 
Utilize constructors for initialization, accessors for retrieval, mutators for modification, and override equals and toString for custom behavior in your classes.
