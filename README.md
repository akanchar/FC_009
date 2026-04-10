# FC 009

This challenge can be worked on in pairs of 2 and the focus for this challenge is on the topics we covered this week:
1. Installing Unity
2. Getting Unity to make a mobile app
3. Running the mobile app on Unity

## Github Classrooms
We will be using Github classroom to do in-class Friday Challenges.
You can make as many commits and as many pushes as needed to the main branch on your forked copy of the repo.
The notes about commits are still relevant here:
To be consistent, use the same styling for commit messages that was given in the Project I:
- PREFIX – Short description of the change
  A detailed description can be added to the commit in the long description, if needed.
  The following are the possible options for [Prefix]
- [FEAT] - For new features or major additions to the project.
  FEAT - Added button click-ability feature 
- [FIX] - For bug fixes, corrections, or revisions to the code.
  FIX - Corrected navigation bar alignment on mobile devices
- [STYLE] - For stylistic changes such as formatting, CSS modifications, or minor visual updates.
  STYLE - Updated color scheme for better contrast
- [DOCS] - For changes or additions to the documentation, including README files and comments in the code.
  DOCS - Added project description and setup instructions to README
- [SECURITY] - For changes related to improving the security of the website.
  SECURITY - Implemented input validation for contact form
- [REFACTOR] - For code refactoring that doesn’t change functionality but improves code quality or organization.
  REFACTOR - Organized attributes for button components files in Home layout.
- [TEST] - For adding tests or making changes to the testing suite.
  TEST - Added validation tests for login form input

### 5. Submitting your work
Once, you are sure that all the work is completed, go through the following steps for submission.
Push all your work onto the main branch. **Only the main branch** will be considered for grading.

## Project description
The repository is empty and your goal for this challenge is to make a simple unity project and have that run on the Android emulator.
Note that the instructions given here might vary for different machines.

Total points - 38

Task 1 - 3

Task 2 - 5

Task 3 - 5

Task 4 - 10

Task 5 - 10

Task 6 - 5


### Task 1: Create a simple Unity scene with a cube
### Task 2: Make sure that the camera sees the cube.
Select Main Camera, In the Inspector, set Position to something like:

X: 0

Y: 1

Z: -5

The cube should now be visible in the Game view. Double check by clicking on the play button
which will play the scene. Press the Play button to confirm it works.

### Task 3: Set up Unity for Android
Install Android Build Support (if not already)
In Unity Hub:
1. Go to Installs 
2. Click the gear ⚙️ next to your Unity version → Add Modules 
3. Make sure these are checked: Android Build Support  and Android SDK & NDK Tools  and OpenJDK
### Task 4: Switch platform to Android
In Unity, go to:

File -> Build Settings

Select Android

Click Switch Platform (might take a while)

### Task 4: Run on Android Emulator (via Android Studio)
Start your emulator on Android Studio, Go to:
1. Device Manager
2. Manually start an emulator (Pixel, etc.)

Back in Unity
1. Configure build settings 
2. In File -> Build Settings: 
   1. Click Add Open Scenes
   2. Make sure your scene is listed
3. Player Settings ->
   1. Set Company Name + Product Name
   2. Set Minimum API Level (e.g., API 24+ is safe)
### Task 5: Build and Run
In Build Settings
Click Build and Run, this time Unity will:
1. Build the APK
2. Install it on the emulator
3. Launch it



### Task 6: Add a small script
1. Select the cube
2. Click Add Component
2. Add -> Rotator script (or create one):
```using UnityEngine;

public class RotateCube : MonoBehaviour
{
    void Update()
    {
        transform.Rotate(0, 50 * Time.deltaTime, 0);
    }
}
```



