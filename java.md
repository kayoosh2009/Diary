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


