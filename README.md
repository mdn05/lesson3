// Задача 19
// Напишите программу, которая принимает на вход пятизначное число и проверяет,
//является ли оно палиндромом.
// 14212 -> нет
// 12821 -> да
// 23432 -> да
// namespace std;

class Main {
void main()
{
string str = "14212";
bool f = true;

for (int i=0; i < str.Length / 2; i++)
{
    if (str[i] != str[str.Length -1 -i])
    {
        f = false;
        break;
    }
}
if (f == true)
Console.WriteLine("polindrom");
else if (f == false)
Console.WriteLine("no polindrom");    
}
}


// Задача 21
// Напишите программу, которая принимает на вход координаты двух точек и находит расстояние между ними в 3D пространстве.
// A (3,6,8); B (2,1,-7), -> 15.84
// A (7,-5, 0); B (1,-1,9) -> 11.53

//Формула вычесления расстояния между 3 точками А (xa,ya,za), B(xb,yb,zb)  на плоскостях: S = round(((xb - xa)2 + (yb - ya)2 + (zb - za)2)(1/2), 2)
System.Console.WriteLine ("Ввести xa");
double xa = double.Parse(Console.ReadLine());

System.Console.WriteLine ("Ввести ya");
double ya = double.Parse(Console.ReadLine());

System.Console.WriteLine ("Ввести za");
double za = double.Parse(Console.ReadLine());

System.Console.WriteLine ("Ввести xb");
double xb = double.Parse(Console.ReadLine());

System.Console.WriteLine ("Ввести yb");
double yb = double.Parse(Console.ReadLine());

System.Console.WriteLine ("Ввести zb");
double zb = double.Parse(Console.ReadLine());

double x = Math.Sqrt(Math.Pow(xb - xa, 2) + Math.Pow(yb - ya, 2) + Math.Pow(zb - za, 2));

System.Console.WriteLine(x);

// Задача 23

// Напишите программу, которая принимает на вход число (N) и выдаёт таблицу кубов чисел от 1 до N.
// 3 -> 1, 8, 27
// 5 -> 1, 8, 27, 64, 125


System.Console.WriteLine ("Ввести N: ");
int x = int.Parse(Console.ReadLine());

for (int i = 1; i <= x; i++)
{
    if (i == x)
    {
        System.Console.WriteLine(i * i * i);
        break;
    }
    System.Console.Write(i * i + ", ");
}
