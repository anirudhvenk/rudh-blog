---
layout: post
title:  "Object Oriented Pancakes"
date:   2020-12-30
---
In many ways, I feel as though cooking is a lot like coding. Object oriented coding in specific. Object Oriented Programming helps to keep your code less repetitive making it simpler to manage and support going forward.

Many times have I found myself digging through old photos and handwritten notes of recipes to find a specific one for a dish I plan to cook. You may be familiar with this situation as well; trying to find the recipe you want from the 2-inch-thick stack of recipes can be difficult.

Wouldn’t it be easier if your recipes were in organized binders and grouped together so they are easier to find? The binder organization could be anyway that makes sense to you. For this example, we could sort recipes in binders called appetizers, entrees, desserts, side dishes, etc. Now that everything is organized, it is easier to find those recipes.

The idea is that when you learned to program, you probably wrote everything that you wanted the program to do. As you became more acquainted with programming and what you could do, you noticed your programs became much larger and you were replicating data structures and functionality (maybe even copy and pasting).

In this way, cooking mirrors many of the technalicalities of coding, and I will describe the three core ways it does so: encapsulation, inheritance, and polymorphism.

### Encapsulation

Encapsulation is how OOP starts to help you organize your code. Think of the binders as a class. Inside the binder is everything it means to be an appetizer, entree, or dessert. When you start to look at every recipe there are a lot of commonalities. Every dish has ingredients and all dishes have instructions as well. These can be modeled as fields and functions respectively.

We can use the example of pancakes for this, as the base recipe for a pancake is relatively simple but can have many variations as well.

```java
public class Pancake {
    private Ingredient flour;
    private Ingredient buttermilk;
    private Ingredient egg;
    // other ingredients...

    public void mix(Ingredient flour, Ingredient buttermilk) {
        // mix ingredients together...
    }
}
```

### Inheritance

It’s nice that we have this basic pancake. However, maybe you want to extend your salad to chocolate chip pancakes. In this way, you don’t have to create another constructor class from scratch. 

```java
public class  ChocoChipPancake extends Pancake {
    public ChocoChipPanicake() {
        super();
        // whatever else to do to construct ChocoChipPancake...
    }

    // other ChocoChipPancake specific methods...
}
```

### Polymorphism

One more core concept of programming we can implement is the idea of polymorphism, where you would “morph” an existing class into a new class.

```java
public class ChocoChipPancake extends Pancake {
    public ChocoChipPancake() {
        super("chocolateChips");
        // whatever else to do to construct ChocoChipPancake...
    }

    // other ChocoChipPancake specific methods...
}
```

---
<br>

<p align="center">
  <img src="/images/pancakes/pancakes1.jpeg" width="40%" />
  <img src="/images/pancakes/pancakes2.jpeg" width="40%" />
</p>