Напишите программу, которая на вход принимает позиции элемента в двумерном массиве, и возвращает значение этого элемента или же указание, что такого элемента нет.

Например, задан массив:

1 4 7 2

5 9 2 3

8 4 2 4

1, 7 -> такого элемента в массиве нет



Console.WriteLine("Введите номер строчки ");
int n = Convert.ToInt32(Console.ReadLine());

Console.WriteLine("Введите номер столбца ");
int m = Convert.ToInt32(Console.ReadLine());

int [,] numbers = new int [10,10];
FillArrayRandomNumbers(numbers);

if (n > numbers.GetLength(0) || m > numbers.GetLength(1))
{
    Console.WriteLine("такого элемента нет");
}
else
{
    Console.WriteLine($"значение элемента {n} строки и {m} столбца равно {numbers[n-1,m-1]}");
}

PrintArray(numbers);

void FillArrayRandomNumbers(int[,] array)
{
    for (int i = 0; i < array.GetLength(0); i++)
        {        
            for (int j = 0; j < array.GetLength(1); j++)
            {
                array [i,j] = new Random().Next(-100, 100)/10;
            }   
        }
}

void PrintArray(int[,] array)
{
    for (int i = 0; i < array.GetLength(0); i++)
    {
        Console.Write("[ ");
        for (int j = 0; j < array.GetLength(1); j++)
        {
            Console.Write(array[i,j] + " ");
        }   
        Console.Write("]");
        Console.WriteLine(""); 
    }
}



Введите номер строчки 
1
Введите номер столбца 
9
значение элемента 1 строки и 9 столбца равно -5
[ -5 4 2 -6 -1 -7 9 5 -5 -5 ]
[ -3 6 -4 -2 -4 9 -8 9 4 8 ]
[ -5 -9 6 7 0 -8 0 -6 -1 2 ]
[ 1 -4 3 8 -2 -3 8 6 -9 3 ]
[ 1 -5 9 1 0 0 3 5 9 -5 ]
[ 6 0 -1 -6 7 0 2 7 2 -5 ]
[ 5 8 7 -7 8 0 -2 -2 4 9 ]
[ 9 -1 -6 8 0 -9 6 -9 -3 2 ]
[ -9 0 -9 6 9 -2 5 0 4 3 ]
[ -4 6 -2 -8 7 2 0 -3 -5 2 ]
