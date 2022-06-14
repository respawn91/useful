В данном файле будут приведены популярные задачи по программирования с собеседований тестеров и автотестеров

Факториал

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
