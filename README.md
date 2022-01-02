# Unity_PlayerPrefsExtensions
Easy solution to use bools in PlayerPrefs. Add it to your project and save true or false values with this static class.

## Easy to use in your project
```C#
public class YourClass
{
    void DoSomething()
    {
        if(PlayerPrefsExtension.GetBool("Something"))
        {
            //Something is True
        }
        else
        {
            //Something is False 
        }
    }

    void DoOtherThing()
    {
        //Set starting values to bool, in this case, "OtherThing" default value will be true
        if(PlayerPrefsExtension.GetBool("OtherThing", true))
        {
            //OtherThing is True
            PlayerPrefsExtension.SetBool("AnotherThing", false);
        }
        else
        {
            //OtherThing is False 
            PlayerPrefsExtension.SetBool("AnotherThing", true);
        }
    }
}
```
