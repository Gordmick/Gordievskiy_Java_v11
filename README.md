## Gordievskiy_Java_v11
## Задания, необходимо написать код:

### 1. Составить алгоритм: если введенное число больше 7, то вывести “Привет”  
Решение:
```java
package test_taks;
import java.util.Scanner;
public class task_1 {
    public static void main(String[] args) {
        System.out.println("Введите число");
        Scanner scanner = new Scanner(System.in);
        int number = scanner.nextInt();
        if (number > 7)  {
            System.out.println("Привет");
        }
    }
}
```
### 2. Составить алгоритм: если введенное имя совпадает с Вячеслав, то вывести “Привет, Вячеслав”, если нет, то вывести "Нет такого имени" 
Решение:
```java
package test_taks;
import java.util.Scanner;
public class task_2 {
    public static void main(String[] args) {
        System.out.println("Введите имя");
        String name = "Вячеслав";
        Scanner console = new Scanner(System.in);
        String input_name = console.nextLine();
        if (name.equals(input_name)){
            System.out.println("Привет, Вячеслав");
        } else {
            System.out.println("Нет такого имени");
        }
    }
}
```
### 3. Составить алгоритм: на входе есть числовой массив, необходимо вывести элементы массива кратные 3 
Решение:
```java
package test_taks;
import java.util.Scanner;
public class task_3 {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.println("Введите длину массива:");
        int length = input.nextInt();
        int array[] = new int[length];
        System.out.println("Введите элементы массива:");
        for (int i = 0; i < length; i++) {
            array[i] = input.nextInt();
            if ((array[i] % 3 == 0) && (array[i] != 0)) {
                System.out.print(array[i] + " ");
            }

        }
        System.out.print("- элементы массива кратные 3");
    }
}
```
### 4. Задание, ответ в текстовой форме:  
  Дана скобочная последовательность: [((())()(())]]  
  - Можно ли считать эту последовательность правильной?  
  - Если ответ на предыдущий вопрос “нет” - то что необходимо в ней изменить, чтоб она стала правильной?  
