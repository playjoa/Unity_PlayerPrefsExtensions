# Unity_PlayerPrefsBool
Easy solution to use bools in PlayerPrefs. Add it to your project and save true or false values with this static class.

OBS: Default value is false. You can use PlayerPrefsBool.GetBool("yourPlayerPrefsKey", true); if you wish to use true as the starting value. 

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
        if(PlayerPrefsBool.GetBool("OtherThing", true))
        {
            //OtherThing is True
            PlayerPrefsBool.SetBool("AnotherThing", false);
        }
        else
        {
            //OtherThing is False 
            PlayerPrefsBool.SetBool("AnotherThing", true);
        }
    }
}
```
