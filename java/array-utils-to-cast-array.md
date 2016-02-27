# Java cast primitive arrays and primitive wrapper arrays

> Before talk about ArrayUtils library lets remember some concepts:

* You can't cast differents wrapper types because they are a Objects
* For number wrapper types you can always use base class 'Number' methods. For instance:

```java
Double d = new Double(2.5);
int i = d.intValue();
```

* Equal wrapper and primitive types (as Double and double) can be casted implicitly

```java
double dm = new Double(1);
```

* Is impossible cast differents wrapper and primitive types, also explicitly

```java
//This line will crash
int im = (int) new Double(0);
```

---

### To cast primitive arrays and wrapper arrays use ArrayUtils library from apache



```java

import org.apache.commons.lang.ArrayUtils;

ArrayUtils.toPrimitive(Boolean[] array);
ArrayUtils.toObject(boolean[] array)
```
