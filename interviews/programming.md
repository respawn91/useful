В данном файле будут приведены популярные задачи по программирования с собеседований тестеров и автотестеров

## Алгоритмы

### Циклы

#### Факториал числа.
Необходимо рассчитать факториал натурального числа n
* Решить через цикл
* Решить через рекурсию

#### Фибоначчи
Необходимо рассчитать n-ый член последовательности Фибоначчи
* Решить через цикл
* Решить через рекурсию

### Работа со строками

#### Определить, являются ли две строки анаграммами друг другу

#### Проверить, являются ли два слова (строки) анаграммами друг другу

### Массивы

#### Даны три неубывающих массива чисел. Найти число, которое присутствует во всех трех массивах.
<details>
<summary>Решение</summary>

    public class HelloWorld{

    public static void main(String []args){
    
        int[] array1 = {1,2,4,5};
        int[] array2 = {3,3,4};
        int[] array3 = {2,3,4,5,6};
        
        for(int i = 0; i < array1.length; i++)
        {
            for(int j = 0; j < array2.length; j++)
            {
                for(int k = 0; k < array3.length; k++)
                {
                    if((array1[i] == array2[j]) && (array1[i] == array3[k]))
                    {
                        System.out.println(array1[i]);
                        break;
                    }
                 }
              }
            }
          }
        }

</details>
                                                 
#### Дан массив строк. Найти самое длинное слово в нем.
<details>
<summary>Решение</summary>
    
    public class Main {

        public static String findLongestWord(String[] array) {

          int max = 0;
          int index = 0;

          for(int i = 0; i < array.length; i++) {
            if(array[i].length() > max) {
              index = i;
              max = array[i].length();
            }
          }

          return array[index];

        }

        public static void main(String[] args) {

          String[] array1 = {"Test", "Anton", "Chicago", "Low"};
          String[] array2 = {"", "", "", ""};

          System.out.println(findLongestWord(array1));
          System.out.println(findLongestWord(array2));

      }
    }

</details>    
## ООП

### Стэк
Реализовать свой стэк с функциями положить элемент, достать элемент, напечатать стэк, найти длину стэка.

### Очередь
Реализовать свою очередь с функциями положить элемент, достать элемент, напечатать очередь, найти длину очереди.
