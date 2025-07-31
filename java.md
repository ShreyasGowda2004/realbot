🔷 What is Java?
Java is a high-level, object-oriented, platform-independent programming language developed by James Gosling at Sun Microsystems in 1995 (now owned by Oracle).

🧠 Key Concepts
Concept	Description
JVM (Java Virtual Machine)	Executes Java bytecode, enabling platform independence.
JRE (Java Runtime Environment)	Provides libraries + JVM for running Java apps.
JDK (Java Development Kit)	Full kit including JRE + development tools like javac.
OOP Principles	Inheritance, Polymorphism, Encapsulation, Abstraction.
Multithreading	Java has built-in support for concurrent programming using threads.

📦 Popular Java Libraries & Frameworks
Type	Tools
Web Frameworks	Spring Boot, Jakarta EE, JSF
Testing	JUnit, TestNG, Mockito
Build Tools	Maven, Gradle
UI Frameworks	JavaFX, Swing
ORM	Hibernate

📈 Real-World Usage
Domain	Use Case
Enterprise Apps	Banks, healthcare, insurance systems (e.g., Spring Boot REST APIs).
Android Apps	Java was the original Android development language.
Big Data	Tools like Apache Hadoop use Java.
Embedded Systems	Set-top boxes, sensors, etc.
Scientific Apps	MATLAB plugins, simulation tools.

🔢 Market Data (2025 Estimates)
💻 Used by ~10 million developers globally.

🔄 Over 35 billion Java-enabled devices worldwide.

🏢 Top companies using Java: Amazon, Google, Netflix, Uber, Accenture, Infosys, IBM.

📊 Still among the Top 5 languages in developer surveys (e.g., Stack Overflow, TIOBE Index).

📚 Sample Code (Hello World)
java
Copy
Edit
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
🧩 Key Java Versions
Version	Notable Feature
Java 8	Lambda expressions, Stream API
Java 11 (LTS)	Improved garbage collection, HTTP Client API
Java 17 (LTS)	Sealed classes, enhanced switch
Java 21 (LTS, 2023)	Virtual threads (Project Loom), record patterns
✅ Java Code – Bubble Sort (Ascending Order)
java
Copy
Edit
public class BubbleSort {
    public static void main(String[] args) {
        int[] arr = {64, 25, 12, 22, 11};

        bubbleSort(arr);

        System.out.println("Sorted array:");
        for (int value : arr) {
            System.out.print(value + " ");
        }
    }

    public static void bubbleSort(int[] arr) {
        int n = arr.length;
        boolean swapped;

        // Outer loop for each pass
        for (int i = 0; i < n - 1; i++) {
            swapped = false;

            // Inner loop for pairwise comparison
            for (int j = 0; j < n - 1 - i; j++) {
                // Swap if elements are in wrong order
                if (arr[j] > arr[j + 1]) {
                    // swap arr[j] and arr[j+1]
                    int temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;

                    swapped = true;
                }
            }

            // If no swaps happened in this pass, array is sorted
            if (!swapped) break;
        }
    }
}
