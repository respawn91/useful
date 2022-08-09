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
<details>
<summary>Решение</summary>
    
public class Main {
    
    public static boolean isAnagram(String s1, String s2) {
      
      boolean result = false;
      
      s1 = (s1.toLowerCase()).trim();
      char[] s1Array = s1.toCharArray();
      
      s2 = (s2.toLowerCase()).trim();
      char[] s2Array = s2.toCharArray();
      
      if(s1Array.length != s2Array.length) {
        result = false;
      }
      else {
        Arrays.sort(s1Array);
        Arrays.sort(s2Array);
        
        if(Arrays.equals(s1Array, s2Array) == true)
          result = true;
        else
          result = false;
        }
      return result;
    }
    
    public static void main(String[] args) {
      
      String s1 = "anton";
      String s2 = "noant";
      String s3 = "antan";
      String s4 = "ANTON";
      String s5 = "antony";
      
      System.out.println(isAnagram(s1, s2));  //  true
      System.out.println(isAnagram(s1, s3));  //  false
      System.out.println(isAnagram(s1, s4));  //  true
      System.out.println(isAnagram(s1, s5));  //  false
  }
}

</details> 

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
