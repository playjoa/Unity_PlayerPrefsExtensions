# Unity_PlayerPrefsBool
Easy to implement PlayerPrefsBool static class. Add it to your project and save true or false values with this static class.


## Easy to use in your project
```C#
public class YourClass
{
    void DoSomething()
    {
        if(PlayerPrefsBool.GetBool("Something"))
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
        //Set starting values to bool, in this case, "OtherThing" default value will be false
        if(PlayerPrefsBool.GetBool("OtherThing", false))
        {
            //OtherThing is True
        }
        else
        {
            //OtherThing is False 
        }
    }
}
```
