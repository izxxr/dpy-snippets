# Contributing to dpy-snippets
First things first, Thank you for showing interest in contributing to dpy-packages. 👍

## Snippet suggestions
Suggestions for a new snippet or improvement to an existing snippet are submitted using [GitHub issues](https://github.com/izxxr/dpy-snippets/issues). When
submitting a suggestion make sure to:

- Describe the snippet
- Provide example template code for snippet
- Discuss the use cases

When suggestion an improvement, you should also discuss on why the improvement could be benificial.

## Adding a new snippet
You can also open pull requests for adding new snippets or improving an existing one. In order to add a snippet, you would have to clone this repository
and edit the [`snippets/snippets.code-snippets`](https://github.com/izxxr/dpy-snippets/blob/main/snippets/snippets.code-snippets) file.

Add a new entry in this file of this format:
```code-snippets
{
  "Snippet title": {
    "prefix": ["dpy.prefix"]  // Prefix is self explanatory. You can add more than one prefixes too.
    "body": [  // Body is the actual snippet code (See information below this codeblock for more info)
      "def foo():",
      "\tprint('hello')",  // '\t' adds an indent
    ],
    "description": "Description of this code snippet.",
  }
}
```

- `prefix` is the list of prefixes that user will type to generate the snippet.
- `body` is the list of snippet code lines.
- `description` is the code snippet's description

### Writing Snippet Body
There are many techniques used for writing a snippet's body.

- `\t` adds an indent
- `\n` adds a new line

You should not add indents manually as `\t` tells the editor to add indentation according to how user has configured their indentation
settings such as spaces counts.

A dollar sign with a number is used to indicate the cursor position in the snippet, this allows user to use <kbd>Tab</kbd> to navigate
through the snippet and customize it. For example:
```code-snippets
{
  "Snippet": {
    ...
    "body": [
      "def ${1:foo}($2):",
      "\t$3",
    ]
    ...
  }
}
```
In the above example, snippet cursor position starts from `$1`, where user will write the function name. Note how this point is wrapped in `{}` with dollar
sign outside -- this sets a "default" to this cursor point, by default `foo` will be selected and user can either replace it or choose to navigate to next
cursor point.

After writing the function name, pressing <kbd>Tab</kbd> will move the cursor inside the `()` where user will include the parameters list.
Finally, <kbd>Tab</kbd> will move the cursor inside the function's body.

For more information, read the [VSCode Snippets Guide](https://code.visualstudio.com/api/language-extensions/snippet-guide) or take inspiration
from existing snippets in the file.

### The Golden Rule of Contributing
The only rule for contributing to the repository is to remain consistent with the existing style of code. By consistency, we mean that you should
keep the snippet prefixes similar to existing prefixes. Consistency is the best practice! 🚀
