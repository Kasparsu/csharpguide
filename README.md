* variables
* strings
* datetime
* arrays
* lists
* sets
* dictionaries
* loops
* enums
* objects


# Variables

declared with type, name and optional value

```
type name = value;
```

different simple types are 
* `int` - all full numbers negative and positive
* `float` - all floating point numbers up to 32 bit (7 digits)
* `double` - all floating point numbers up to 64 bit (15-16 digits)
* `decimal` - all floating point numbers up to 128 bit (28-29 significant digits)
* `char` - single character 
* `string` - text, multiple characters, is also taken as char array
* `boolean` or `bool` - truth value or binary value of single bit. can be `true` or `false`
* `array` - list of elements with predefined length
* `object` or `enum` - any object or enum is a type
* `list<type>` - list of certain type, can be any length
* `set<type>` or `hashset` etc - contains list of unique values. no repeats are inserted.
* `dictionary<type, type>` - key, value list that can have a key value tied to value.

##Examples

```
int iNum = 3;
float fNum = 1.4;
double dblNumber = 1.4;
decimal decNumber = 1.4;
char letter = 'a'; // is important to note thet char type is defined between single quotation marks
string text = "Hello World";
bool isLie = false;
int[] arr = {1,2,3};
DateTime time = DateTime.Now;
List<int> numList = new List<int>();
Set<int> numSet = new Set<int>();
Dictionart<string, int> = new Dictionary<string, int>();
```

## Operations

* `num = 1;` assignment, sets value to variable
* `num += 1;` addition, adds value to variable
* `num -= 1;` subtraction, subtracts value from variable
* `num /= 2;` division ...
* `num *= 2;` multiplication ...
* `num++;` increment by one
* `num--;` decrement by one

#Strings

Strings have many operations that can be performed on them.
Most notable are.

* `Clone()` 	Make clone of string.
* `CompareTo()` 	Compare two strings and returns integer value as output. It returns 0 for true and 1 for false.
* `Contains()` 	The C# Contains method checks whether specified character or string is exists or not in the string value.
* `EndsWith()` 	This EndsWith Method checks whether specified character is the last character of string or not.
* `Equals()` 	The Equals Method in C# compares two string and returns Boolean value as output.
* `GetHashCode()` 	This method returns HashValue of specified string.
* `GetType()` 	It returns the System.Type of current instance.
* `GetTypeCode()` 	It returns the Stystem.TypeCode for class System.String.
* `IndexOf()` 	Returns the index position of first occurrence of specified character.
* `ToLower()` 	Converts String into lower case based on rules of the current culture.
* `ToUpper()` 	Converts String into Upper case based on rules of the current culture.
* `Insert()` 	Insert the string or character in the string at the specified position.
* `IsNormalized()` 	This method checks whether this string is in Unicode normalization form C.
* `LastIndexOf()` 	Returns the index position of last occurrence of specified character.
* `Length` 	It is a string property that returns length of string.
* `Remove()` 	This method deletes all the characters from beginning to specified index position.
* `Replace()` 	This method replaces the character.
* `Split()` 	This method splits the string based on specified value.
* `StartsWith()` 	It checks whether the first character of string is same as specified character.
* `Substring()` 	This method returns substring.
* `ToCharArray()` 	Converts string into char array.
* `Trim()` 	It removes extra whitespaces from beginning and ending of string.
 
```

    using System.Text;
    namespace string_function
    {
        class Program
        {
            static void Main(string[] args)
            {
                string firstname;
                string lastname;
               
               
                firstname = "Steven Clark";
                lastname = "Clark";
     
     
      Console.WriteLine(firstname.Clone());
    // Make String Clone
                Console.WriteLine(firstname.CompareTo(lastname));
    //Compare two string value and returns 0 for true and
    1 for false
     
     Console.WriteLine(firstname.Contains("ven")); //Check whether specified value exists or not in string
     
      Console.WriteLine(firstname.EndsWith("n")); //Check whether specified value is the last character of string
                Console.WriteLine(firstname.Equals(lastname));
    //Compare two string and returns true and false
     
     
      Console.WriteLine(firstname.GetHashCode());
    //Returns HashCode of String
     
      Console.WriteLine(firstname.GetType());
    //Returns type of string
     
      Console.WriteLine(firstname.GetTypeCode());
    //Returns type of string
     
      Console.WriteLine(firstname.IndexOf("e")); //Returns the first index position of specified value
    the first index position of specified value
     
      Console.WriteLine(firstname.ToLower());
    //Covert string into lower case
     
      Console.WriteLine(firstname.ToUpper());
    //Convert string into Upper case
     
      Console.WriteLine(firstname.Insert(0, "Hello")); //Insert substring into string
     
      Console.WriteLine(firstname.IsNormalized());
    //Check Whether string is in Unicode normalization
    from C
     
     
       Console.WriteLine(firstname.LastIndexOf("e")); //Returns the last index position of specified value
     
     Console.WriteLine(firstname.Length);
    //Returns the Length of String
     
     Console.WriteLine(firstname.Remove(5));
    //Deletes all the characters from begining to specified index.
     
     Console.WriteLine(firstname.Replace('e','i')); // Replace the character
     
      string[] split = firstname.Split(new char[] { 'e' }); //Split the string based on specified value
     
     
                Console.WriteLine(split[0]);
                Console.WriteLine(split[1]);
                Console.WriteLine(split[2]);
     
      Console.WriteLine(firstname.StartsWith("S")); //Check wheter first character of string is same as specified value
     
      Console.WriteLine(firstname.Substring(2,5));
    //Returns substring
     
      Console.WriteLine(firstname.ToCharArray());
    //Converts an string into char array.
     
      Console.WriteLine(firstname.Trim());
    //It removes starting and ending white spaces from
    string.
               
            }
        }
    }
```

# Datetime

https://docs.microsoft.com/en-us/dotnet/api/system.datetime?view=netcore-2.2#methods

# Arrays

Arrays are way to keep values in a list which lenght is known from start.

