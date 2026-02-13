[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/pOLhHg-2)
# FC 003
This challenge can be worked on in pairs of 2.
Focus for this challenge is on the topics we covered this week:
1. Navigation
2. Fragments
3. Fragment Container
4. SupportManager / FindNavController
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
Various layouts defining a scenario from the first mission in a famous game titled - **Detroit Become Human** are provided to you.
Your goal is to arrange all the fragments in an appropriate order so that all the transitions 
are meaningful.

Note that you **are not supposed** to add any widgets or any layouts, unless explicitly specified (Task #1).

### Task 1: Add a FragmnetContainerView to the activity_main.kt
In order for the fragments to show on the UI, we need a fragment contianer view layout to hold 
all the fragments. Make sure to add a fragment container view to the activity_main.kt.
### Task 2: Add a navigation resource folder and a nav.xml resource file
A navigation resource folder needs to be added to teh res folder in Android Studio.
Once the folder is added, add a navigation resource file and name is nav.xml
### Task 3: Arrange the layouts accordingly
In the nav.xml file, arrange all the fragments depending on how you think is the appropirate order.
Note that there should not be any fragments that are unreachable.

And yes, the fragments do not have proper naming conventions and this is on purpose, although 
it is a bad programming practice.

Every fragment should be reachable in atleast one way. The "Replay Mission" button should redirect to the start of the nav.xml
### Task 4: Add the button onclick Listeners
Every button in each fragment should have an on-click listener, which will contain 
the logic to change the fragments. Note that fragments can be changed using the follwing command:

`findNavController().navigate(R.id.action_fragment1_to_fragment2)`
### Task 5: Replay mission button should not enable back button
When the replay mission is clicked, make sure the fragment cannot go back and takes
the user to the home screen to restart the game. 
Look for the following attributes in nav.xml file to handle the back button characteristics:
1. popUpTo="@id/fragment1"
2. popUpToInclusive="true"

**Make sure to test that your app runs after making all the above changes**