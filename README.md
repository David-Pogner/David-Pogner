```csharp
using System;

namespace HTBLA_Leonding
{
    class ProgrammerStudent
    {
        public string Name { get; set; }
        public string School { get; set; }
        public string[] ProgrammingLanguages { get; set; }

        public void Introduce()
        {
            Console.WriteLine($"Hi, I'm {Name}, a passionate programmer studying at {School}.");
        }

        public void DisplayLanguages()
        {
            Console.WriteLine($"I am proficient in the following programming languages: {string.Join(", ", ProgrammingLanguages)}.");
        }

        static void Main(string[] args)
        {
            ProgrammerStudent student = new ProgrammerStudent
            {
                Name = "David",
                School = "HTBLA Leonding",
                ProgrammingLanguages = new[] { "C#", "C++" }
            };

            student.Introduce();
            student.DisplayLanguages();
        }
    }
}
```
