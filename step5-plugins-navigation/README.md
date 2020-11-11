# React Native

## Step 5 - Plugins - Navigation

> 📘 React Native docs - [Navigating between screens](https://reactnative.dev/docs/navigation)

There are several navigation plugins that you can use, however, you probably want [React Navigation](https://reactnavigation.org/.

### Before Each

Install [React Navigation](https://reactnative.dev/docs/navigation#installation-and-setup).

### Task 1 - Tab Navigation

Create a Tab Navigator UI.

```
Routes:
- Default route: Home (/)
- Route: Posts (/posts)
```

Requirements:

- Tabs displayed "Home" and "Posts"
- From Home, a user can tap the Posts Tab to navigate to Posts route.
- From Posts, a user can tap the Home Tab to navigate to Home route.

### Task 2 - Stack Navigation

Create a Stack Navigator UI.

```
Routes:
- Default route: Posts (/)
- Route: Post (/posts/\$id)
```

Requirements:

- There is no Tab navigation
- From Posts, a user can tap a post to open Post
- Post route displays post id
- Post route, has a link at top "Back", when tapped navigates the user back to Posts

### Task 3 - Mixed (Tab, Stack)

This task builds on Task 1 and Task 2. The task is to create a Tab Navigator with a nested Stack Navigator.

```
Routes:
- Default route: Home (/)
- Route: Posts (/posts)
- Route: Post (/posts/\$id)
```

Requirements:

- Requirements from Task 1 and Task 2
- Tab navigation includes only "Home" and "Posts"

### Task 3 - Drawer Navigation

Create a Drawer Navigator UI.

```
Routes:
- Default route: Home (/)
- Route: Settings (/settings)
- Route: About (/about)
```

Requirements:

- Each route includes a link "Open", when tapped opens the navigation drawer

### Task 4 Mixed (Tab, Stack, Drawer)

This task builds on all of the above tasks. The task is to create a Drawer Navigator, with a nested Tab Navigator, which has a nested Stack Navigator.

```
Routes:
- Default route: Home (/)
- Route: Posts (/posts)
- Route: Post (/posts/\$id)
- Route: Credits (/credits)
- Route: Settings (/settings)
- Route: About (/about)
```

Requirements:

- Drawer navigation items should display "Home", "Settings" and "About"
- Tab navigation items should display "Posts", "Credits"
- Posts and Post behaviour is the same as Task 2

### Task 5 - Onboarding flow

Create an app that when opened launches a 3 screen Onboarding Flow. After the Onboarding Flow, open Home.

On Home, there should be Tabs "Home" and "About".

```
Routes:
- Route: Onboarding (/onboarding/\$id)
- Default route: Home (/)
- Route: About (/about)
```

Verify this works by hard-coding a flag `hasOnboarded`, toggle this to true or false and test it is working by force closing and reopening the app. If the user has onboarded, the expectation is that the app should start from Home, else the app should start from Onboarding.
