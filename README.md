// Напишите программу, которая принимает на вход пятизначное число и проверяет, является ли оно палиндромом.
//14212 -> нет
//12821 -> да
//23432 -> да

Console.WriteLine("Введите длину числа: ");

int n = Convert.ToInt32(Console.ReadLine());

Console.WriteLine($"Введите {n} цифр числа по одному: ");

int[] a = new int[n];

for (int i =0; i<n; i++)

{
    a[i] = Convert.ToInt32(Console.ReadLine());
}

int j = 0;

int k = n-1;

bool flag = true;

while ( j<k )
{

  if (a[j] != a[k])
  
  {
  
    flag = false;
    
  }
  
  j++;
  
  k--;
  
}

if (flag == true)

{
    Console.WriteLine("Число является палиндромом");
}

else

{
    Console.WriteLine("Число не является палиндромом");
}
