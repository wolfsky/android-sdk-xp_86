Developing AOSP App from Android SDK

1.Installing debug library that contains hidden or internal classes
    (1) git clone android-sdk-xp_86 from github

2.Add user libraries (android-sdk-xp_86\platforms\android-2.1)
    (1) Open eclipse / Preference / Java / Build Path / User Libraries / @New
    (2) Enter any names you want, and click OK to add.
    (3) Select the libraries you added, and press @Add JARs...
    (4) Add all libraries JARs from libraries copied from step 1.2

3.Import AOSP apps to Eclipse
    (1) Copy app folder from Android Source to wherever you like (I don't like my android source messed up)
    (2) Create New Android Project from eclipse.
    (3) Check "Create New Android Project / Contents / Create project from existing source", Browse the app folder you copied at step 3.1.
    (4) Check "Create New Android Project / Build Target / Android 2.1".
    (5) Press @Finish to create new project.

4. Changing default SDK libraries to our full debug libraries.
    (1) Left click project created at Step 3 at Package Explorer, and click "Properties" menu.
    (2) Select stocking "Android 2.1" and click Remove.
    (3) Press "Properties for ${project} / Java Build Path / Libraries / @Add Library".
    (4) Select "Add Library / User Library " and click Next.
    (5) Check libraries we add at Step 2, and click finish.
    (6) Click OK to apply setting.

5. Clean up project by click "Project / Clean / Clean all projects"