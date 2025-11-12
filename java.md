# 12.11.2025 - 
<br> <br> <br> <br> <br>










# 04.11.2025 - Символы и String
Компьютер всегда когда получает данные то они зашифровываются как strung <br>
Так же не стоит забывать что для вызова текста нужно использовать ***scan.nextLine()*** или ***scan.next()*** <br> <br>

***next.Line*** используется для сканирования всей строки а вот <br>
***next()*** для сканирования всего одного слово и он больше не записывает все что было после пробела <br>

Так же есть char который сам по себе является одним символом и его мы сохраняем ввиде 'a' в отличии от string где используется для сохранения  "a" <br>
Так же не многие знаю что для получения такого символа нужно использовать ***scan.next(). charAt(0)***.<br> <br>


Для того чтобы сравнивать string с string, нужно использовать ***equals***

<br> <br> <br> <br> <br>











# 04.11.2025 - if, else & switch
Что такое Switch? <br>
Это помощь для упрощения кода если есть много if и else 

```java
public class TemperatureCheckSwitch {
    public static void main(String[] args) {
        int temperature = 15; // Текущая температура

        System.out.println("Проверяем температуру " + temperature + "°C (используя switch):");

        // Switch может проверять только конкретные значения, что непрактично для температуры.
        switch (temperature) {
            case 0:
                System.out.println("Точка замерзания!");
                break;
            case 15:
                System.out.println("Идеальная комнатная температура.");
                break;
            case 30:
                System.out.println("Уже жарко!");
                break;
            default:
                System.out.println("Температура не является ни одним из предустановленных значений.");
                break;
        }
    }
}
```
Вот как рабоатет switch:
```txt
1. switch ( temperature ) - проверяет данное хранилище в котором хранится температура
2. case 0: - если температура 0 то он выполняет действия ниже указаного case
3. default: - если нету нужного значение выполняется данное действие
4. break; - пишется у каждого кейса для выхода
```
Так же главное запомнить что нельзя использовать break и continue где угодно но только в switch

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        System.out.println("Enter month");
        String num_m = scan.nextLine();

        switch (num_m) {
            case "January":
            case "March":
            case "May":
            case "July":
            case "August":
            case "October":
            case "December":
                System.out.println(31 + " Days");
                break;


            case "April":
            case "June":
            case "September":
            case "November":
                System.out.println(30 + " Days");
                break;

            case "February":
                System.out.println(28+"or"+29 + " Days");
                break;

            default:
                System.out.println("Invalid input");
                break;
        }
    }
}
```
<br> <br> <br> <br> <br>








# 29.10.2025 - if/else

``` java
static void charType()
{
  char letters;
  System.out.println("Please enter a letter: ");
  letter = Input.next().charAt(0);

  if ((letter >= 'a' && letter <= 'z' ) ||
    (letter >= 'A' && letter <= 'Z' ))
    System.out.println ("A letter");
  else if (letter >= '0' && letter <= '9' )
    System.out.println ("Digit");
  else //any symbol
    System.out.println ("Neither letter not a dight");
```
Данный код проверяет введеный символ и выводит информацию что это за символ <br>
У каждой буквы или символа есть свое значение по таблице хаски , и именно по этому мы можем играться с буквами и символами как хотим, запони это так как оно будет очень сильно пользоваться в будущем.
<br> <br> <br> <br> <br>










# 28.10.2025 - if/else
Для добавления if нужно написать if и внутри скобок соответствие на проверку

``` java
if (avg <= 25) {
  System.out.println("It was a warn day");
}
```
В отличии от пайтона мы используем {} а не : так как мы пишем на языке жава

```txt
Операторы которые мы используем для if:
1. < > - маленький большой
2. >= <= - больше или равно и меньше или равно
3. == != - равно или не равно
```

Если ответ на if выводит True то програма выводит то что задано под if <br>
Если нет, то читается то что находится под else.

```txt
Так же в отличии от пайтона нету if, or и not в жаве, стардайте молча ня<br>
1. and - &&
2. or - ||
3. not - !
```
