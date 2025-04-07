# Tests
If you have downloaded an exercise using the exercism CLI, you will have a folder containing the solution function template (which you then edit to create your solution), a test function and some metadata.

## Running Tests
Create a link in the active workspace to the exercise folder:

```
      ]LINK.Create # /path/to/exercise
Linked: # ←→ C:\path\to\exercise
```

You should now see your solution definition and a test function in the workspace:

```
      ]Names
Exercise Test_Exercise
```

Changes made using the Dyalog editor (e.g. with `)ED'Exercise'`) will be automatically updated in the file.

Running the test function will error on the first failure, and should suspend in the tracer where you can view the test case and attempt to fix your solution.

```
      Test_HelloWorld
assertion failure
Test_HelloWorld[5] Assert'Hello, World!'≡HelloWorld ⍬
                   ∧
```

> **NOTE:**
    User commands (expressions that begin with a right square bracket `]`) cannot be used inside APL functions. They are tools for use when developing code in Dyalog. The executable equivalent of the above is `⎕SE.Link.Create # '/path/to/exercise'`.
