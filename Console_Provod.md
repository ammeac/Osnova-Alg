>мозг расплавился

#Задание 1

  ```
using System;
using System.IO;
class program
{
    static void Main(string[] args)
    {
        string dir = Directory.GetCurrentDirectory();
        Console.WriteLine("Сейчас тут: " + dir);
        string[] files = Directory.GetFiles(dir);
        foreach (string file in files)
        {
            Console.WriteLine(file);
        }
        Console.WriteLine("Нажмите любую клавишу для выхода.");
        Console.ReadKey();
    }
}
  ```

#Задание 2
  ```
using System;
using System.IO;

class program
{
    static void Main(string[] args)
    {
        DriveInfo[] drives = DriveInfo.GetDrives();
        foreach (DriveInfo drive in drives)
        {
            Console.WriteLine("Диск: " + drive.Name + " Объем: " + drive.TotalSize);
        }
        Console.WriteLine("Нажмите любую клавишу для выхода.");
        Console.ReadKey();
    }
}

  ```

#Задание 3

  ```

using System;
using System.IO;

class program
{
    static void Main(string[] args)
    {
        Console.Write("Имя файла: ");
        string name = Console.ReadLine();
        Console.Write("тут что-то написано: ");
        string text = Console.ReadLine();
        File.WriteAllText(name, text);
        Console.ReadKey();
    }
}
  ```
