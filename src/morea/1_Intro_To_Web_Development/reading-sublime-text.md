---
title: "Sublime Text tutorial"
published: true
morea_id: reading-sublime-text
morea_summary: "How to set up and use the text editor Sublime Text"
morea_type: reading
morea_sort_order: 4
morea_labels:
 - Sublime Text
 - tutorial
---

# Sublime Text

Sublime Text is a powerful, feature-heavy text editor. Text editors are programs used to write code in plaintext, and are different from word processors (ex. Microsoft Word, Google Docs) because of the lack of formatting and styling.

## Setup

In this portion we are going to go over the setup for your coding environment so you can start coding for this class.

### Downloading Packages

One of the great perks of Sublime Text is their open source plugin library. Plugins are designed for developers by developers to add certain features to Sublime Text.
We are going to get a few basic packages for Sublime Text set up. But before we do we have to get the package manager from [packagecontrol.io](https://packagecontrol.io/installation)

#### Instructions from [Packagecontrol.io](https://packagecontrol.io/installation)

1. Open up the command palette: `Cmd + Shift + P`
2. Paste this code in the in the command palette:  
  `import urllib.request,os,hashlib; h = '2915d1851351e5ee549c20394736b442' + '8bc59f460fa1548d1514676163dafc88'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)`
3. Restart Sublime Text

When finished, we can start downloading packages into Sublime Text.

#### Installing Packages

To download and install packages:
1. `cmd + shift + p` to open the command palette in Sublime
2. Type in `package install` and you should see and highlight the `Package Control: Install Package`
3. Wait for text area to show then type the name of the package you want to install and press enter when found.
4. Restart Sublime Text and you're good to go!

Recommended plugins:
* JSLint - Lints your JavaScript code. Linting finds your syntax errors and sub-optimally written code.
* DocBlockr - Simplifies commenting in JavaScript for both reulgar inline and docblock comments.

### subl shortcut

You can configure your shell to open files and folders easier by creating the `subl` shortcut in Bash.

To set up the subl command in Bash we need to create a symbolic link (a file that references/points to another file).

In your terminal, type in: `ln -s /Applications/Sublime\ Text\ 3.app/Content/SharedSupport/bin/subl /usr/local/bin/subl`

Now you can open any file or directory by inputting the Bash command:
* `subl <file>` - Opens the specified file.
* `subl <filepath>` - Opens the specified path.
* `subl .` - Opens the directory where the command was run.

You can also open files by dragging them from your Finder onto the Sublime Text application icon on the Dock, or by dragging the file directly onto your open Sublime Text window.

If you didn't really understand this section, don't worry. We'll go over the command line and Bash in the next module.

## Editing Files

First open a file from your terminal, finder, or sidebar ("file tree").
Once it's open, simply start typing code. When you're done, save.

You can tell when files have been saved by looking at the tab for the file on the tab bar of your editor.

* If it has a circle next to the name then the file has not been saved.

* If the file has been saved then instead of a circle you should see an X.

Remember, saving files is important. Don't end up being the person who writes a hundred lines of code and then loses it because you didn't save.

## Panels/Workspace Setup

Part of being a good developer is having a good workspace. Sublime Text has tools and shortcuts that help you create a good working environment. One of those tools is the Pane feature.

Panes allow you to work on multiple files at the same time in your editor.

To create a pane go to `VIEW > Panes` and then select the type of split screen you want.

| Screen Split | Shortcut               |
| ------------ | ---------------------- |
| Split Up     | `⌘ + ↑`                |
| Split Down   | `⌘ + ↓`                |
| Split Right  | `⌘ + →`                |
| Split Left   | `⌘ + ←`                |

## Tools/Shortcuts/Keys

* `⌘` : Command key
* `⌃` : Control key
* `⌫` : Delete key
* `↑` : Up arrow key
* `←` : Left arrow key
* `→` : Right arrow key
* `↓` : Down arrow key
* `⌥` : Option or Alt key
* `↩` : Return or Enter key
* `⇧` : Shift key

| Shortcut             | Command               |
| -------------------- | --------------------- |
| Save File            | `⌘ + S`               |
| Save File As         | `⌘ + ⇧ + S`           |
| New File in New Tab  | `⌘ + N`               |
| New Tab              | `⌘ + T`               |
| Open File            | `⌘ + O`               |
| Multiline selector   | `⌥ + mouse drag`      |
| Multiline Selector   | `⌘ + mouse click`     |


### Goto Anything

Use Goto Anything to open files and instantly jump to given lines, words, or symbols in just a few keystrokes.

Invoke Goto Anything with: `⌘ + P`

It is possible to:
* Type part of a file name to open it.
* Type `@` to jump to symbols, `#` to search within the file, and `:` to go to a line number.
* These shortcuts can be combined, so `tp@rf` may take you to a function `read_file within a file text_parser.py`. Similarly, `tp:100` would take you to line 100 of the same file.


## Let's move on

This reading concludes the first module, "Intro to Web Development". Now that you've set up your coding environment for the rest of the class, you're ready to start your journey to become a full-fledged web developer! Begin by moving on to the second module, ["Intro to Command Line"](https://junior-devleague.github.io/JDLA-Web-Development/modules/intro-to-command-line/).
