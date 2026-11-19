19/11/26



COLLECTION FRAMEWORKS:



1.ARRAYLIST

2.HASH SET

3.HASH MAP



Core Interfaces in the Collections Framework

Here are some common interfaces, along with their classes:



**Interface	Common Classes	                     Description**

List	   ArrayList, LinkedList	      Ordered collection that allows duplicates

Set	   HashSet, TreeSet, LinkedHashSet    Collection of unique elements

Map	   HashMap, TreeMap, LinkedHashMap   Stores key-value pairs with unique keys





**Interface**	**Class**	                             **Description**

List	     ArrayList	                  Resizable array that maintains order and allows duplicates

&#x20;            LinkedList	                  List with fast insert and remove operations



Set	       HashSet	                  Unordered collection of unique elements

&#x20;              TreeSet	                Sorted set of unique elements (natural order)

&#x20;              LinkedHashSet	        Maintains the order in which elements were inserted



Map	        HashMap	                 Stores key/value pairs with no specific order

&#x20;                TreeMap	        Sorted map based on the natural order of keys

&#x20;              LinkedHashMap	       Maintains the order in which keys were inserted.





**Array list:**



you can use methods like add(), get(), set(), and remove() to manage your list of elements.



Add Elements

To add elements to an ArrayList, use the add() method:



Example

import java.util.ArrayList;



public class Main {

&#x20; public static void main(String\[] args) {

&#x20;   ArrayList<String> cars = new ArrayList<String>();

&#x20;   cars.add("Volvo");

&#x20;   cars.add("BMW");

&#x20;   cars.add("Ford");

&#x20;   cars.add("Mazda");

&#x20;   System.out.println(cars);

&#x20; }

}



output:

\[Volvo, BMW, Ford, Mazda]



import java.util.ArrayList;



public class Main { 

&#x20; public static void main(String\[] args) { 

&#x20;   ArrayList<String> cars = new ArrayList<String>();

&#x20;   cars.add("Volvo");

&#x20;   cars.add("BMW");

&#x20;   cars.add("Ford");

&#x20;   cars.add("Mazda");

&#x20;   System.out.println(cars.get(0));

&#x20; } 

}



output:

Volvo



**SET:**



Java Set Interface

The Set interface is part of the Java Collections Framework and is used to store a collection of unique elements.



Unlike a List, a Set does not allow duplicates, and it does not preserve the order of elements (unless you're using TreeSet or LinkedHashSet).



Common classes that implement Set:



HashSet - fast and unordered

TreeSet - sorted set

LinkedHashSet - ordered by insertion





Java HashSet

A HashSet is a collection of elements where every element is unique.



It is part of the java.util package and implements the Set interface.



Create a HashSet:

ExampleGet your own Java Server

Create a HashSet object called cars that will store strings:



import java.util.HashSet; // Import the HashSet class



HashSet<String> cars = new HashSet<String>();

Now you can use methods like add(), contains(), and remove() to manage your collection of unique elements.





Java TreeSet

A TreeSet is a collection that stores unique elements in sorted order.



It is part of the java.util package and implements the Set interface.



Tip: Unlike HashSet, which has no order, TreeSet keeps its elements sorted automatically.



Create a TreeSet

ExampleGet your own Java Server

Create a TreeSet object called cars that will store strings:



import java.util.TreeSet; // Import the TreeSet class



TreeSet<String> cars = new TreeSet<>();

Now you can use methods like add(), contains(), and remove() to manage your sorted set of elements.



Add Elements

To add elements to a TreeSet, use the add() method:



Example

import java.util.TreeSet;



public class Main {

&#x20; public static void main(String\[] args) {

&#x20;   TreeSet<String> cars = new TreeSet<>();

&#x20;   cars.add("Volvo");

&#x20;   cars.add("BMW");

&#x20;   cars.add("Ford");

&#x20;   cars.add("BMW");  // Duplicate

&#x20;   cars.add("Mazda");



&#x20;   System.out.println(cars);

&#x20; }

}



OUTPUT:

\[BMW, Ford, Mazda, Volvo]



Java LinkedHashSet

A LinkedHashSet is a collection that stores unique elements and remembers the order they were added.



It is part of the java.util package and implements the Set interface.



Tip: Use LinkedHashSet when you want a set that does not allow duplicates and keeps the original insertion order.



Create a LinkedHashSet

ExampleGet your own Java Server

Create a LinkedHashSet object called cars that will store strings:



import java.util.LinkedHashSet; // Import the LinkedHashSet class



LinkedHashSet<String> cars = new LinkedHashSet<>();

Now you can use methods like add(), contains(), and remove() to manage your collection.



Add Elements

To add elements to a LinkedHashSet, use the add() method:



Example

import java.util.LinkedHashSet;



public class Main {

&#x20; public static void main(String\[] args) {

&#x20;   LinkedHashSet<String> cars = new LinkedHashSet<>();

&#x20;   cars.add("Volvo");

&#x20;   cars.add("BMW");

&#x20;   cars.add("Ford");

&#x20;   cars.add("BMW");  // Duplicate

&#x20;   cars.add("Mazda");



&#x20;   System.out.println(cars);

&#x20; }

}



OUPUT:

\[Volvo, BMW, Ford, Mazda]







**HASH MAP:**



Java Map Interface

The Map interface is a part of the Java Collections Framework and is used to store key-value pairs. Each key must be unique, but values can be duplicated.



A Map is useful when you want to associate a key (like a name or ID) with a value (like an age or description).



Common classes that implement Map:



HashMap - fast and unordered

TreeMap - sorted by key

LinkedHashMap - ordered by insertion



Common Map Methods



Method	            Description

put()	        Adds or updates a key-value pair

get()	        Returns the value for a given key

remove()	Removes the key and its value

containsKey()	Checks if the map contains the key

keySet()	Returns a set of all keys





Java HashMap

A HashMap stores items in key/value pairs, where each key maps to a specific value.



It is part of the java.util package and implements the Map interface.



Instead of accessing elements by an index (like with ArrayList), you use a key to retrieve its associated value.



A HashMap can store many different combinations, such as:



String keys and Integer values

String keys and String values

Create a HashMap

Create a HashMap object called capitalCities that will store String keys and String values:



ExampleGet your own Java Server

import java.util.HashMap; // Import the HashMap class



HashMap<String, String> capitalCities = new HashMap<>();

Now you can use methods like put() to add key/value pairs, get() to retrieve a value by key, and remove() to delete an entry - all by using keys instead of index numbers.



Add Items

To add items to a HashMap, use the put() method:



Example

// Import the HashMap class

import java.util.HashMap;



public class Main {

&#x20; public static void main(String\[] args) {

&#x20;   // Create a HashMap object called capitalCities

&#x20;   HashMap<String, String> capitalCities = new HashMap<String, String>();



&#x20;   // Add keys and values (Country, City)

&#x20;   capitalCities.put("England", "London");

&#x20;   capitalCities.put("India", "New Dehli");

&#x20;   capitalCities.put("Austria", "Wien");

&#x20;   capitalCities.put("Norway", "Oslo");

&#x20;   capitalCities.put("Norway", "Oslo"); // Duplicate

&#x20;   capitalCities.put("USA", "Washington DC");



&#x20;   System.out.println(capitalCities);

&#x20; }

}



OUTPUT:

{Austria=Wien, USA=Washington DC, Norway=Oslo, England=London, India=New Dehli}



Java TreeMap

A TreeMap is a collection that stores key/value pairs in sorted order by key.



It is part of the java.util package and implements the Map interface.



Tip: Unlike HashMap, which does not maintain order, TreeMap keeps its keys sorted.



Create a TreeMap

Create a TreeMap that stores String keys and String values:



ExampleGet your own Java Server

import java.util.TreeMap; // Import the TreeMap class



TreeMap<String, String> capitalCities = new TreeMap<>();

Now you can use methods like put(), get(), and remove() to manage sorted key/value pairs.



Add Items

Use the put() method to add key/value pairs:



Example

import java.util.TreeMap;



public class Main {

&#x20; public static void main(String\[] args) {

&#x20;   TreeMap<String, String> capitalCities = new TreeMap<>();

&#x20;   capitalCities.put("England", "London");

&#x20;   capitalCities.put("India", "New Dehli");

&#x20;   capitalCities.put("Austria", "Wien");

&#x20;   capitalCities.put("Norway", "Oslo");

&#x20;   capitalCities.put("Norway", "Oslo"); // Duplicate

&#x20;   capitalCities.put("USA", "Washington DC");



&#x20;   System.out.println(capitalCities);

&#x20; }

}



OUTPUT:

{Austria=Wien, England=London, India=New Dehli, Norway=Oslo, USA=Washington DC}



Java LinkedHashMap

A LinkedHashMap stores keys and values, and keeps them in the same order you put them in.



It is part of the java.util package and implements the Map interface.



Tip: Use LinkedHashMap when you want predictable iteration order (insertion order).



Create a LinkedHashMap

Create a LinkedHashMap object called capitalCities that will store String keys and String values:



ExampleGet your own Java Server

import java.util.LinkedHashMap; // Import the LinkedHashMap class



LinkedHashMap<String, String> capitalCities = new LinkedHashMap<>();

Now you can use methods like put() to add key/value pairs, get() to retrieve a value by key, and remove() to delete an entry - all while maintaining insertion order.



Add Items

Use the put() method to add items to the LinkedHashMap:



Example

// Import the LinkedHashMap class

import java.util.LinkedHashMap;



public class Main {

&#x20; public static void main(String\[] args) {

&#x20;   LinkedHashMap<String, String> capitalCities = new LinkedHashMap<>();



&#x20;   capitalCities.put("England", "London");

&#x20;   capitalCities.put("India", "New Dehli");

&#x20;   capitalCities.put("Austria", "Wien");

&#x20;   capitalCities.put("Norway", "Oslo");

&#x20;   capitalCities.put("Norway", "Oslo"); // Duplicate

&#x20;   capitalCities.put("USA", "Washington DC");



&#x20;   System.out.println(capitalCities);

&#x20; }

}



Output: The items will appear in the order they were added (e.g., {England=London, India=New Dehli, Austria=Wien, Norway=Oslo, USA=Washington DC}).



Note: Duplicates like "Norway" are ignored.



