# Sublime Text 2 plugin: Goto Documentation

A command to jump to documentation for the current word.

## ihowson branch

This branch improves the Python documentation lookup.

I don't like `help()` style docs, so (with configuration) lookups will go to the HTML documentation. If it's not configured or a suitable page can't be found, it'll do a search on doc.python.org.

You should download the Python documentation library ([Python 2](http://docs.python.org/2/download.html) or [Python 3](http://docs.python.org/3/download.html)). Tweak your config to set the path where you've unzipped this:

    "goto_documentation_python_path": "/Users/Ian/Documents/python-2.7.3-docs-html"

## Supports

 * PHP
 * JS / CoffeeScript
 * Python
 * Clojure
 * Go
 * Smarty
 * Ruby on Rails

Submit a patch adding more and I'll include it.

## Using

Open the command palette (cmd-shift-p) and choose "Goto Documentation" while your cursor is on a word.

Make a keybind by adding the following to your `User/Default (OSX).sublime-keymap`:

	{ "keys": ["super+shift+h"], "command": "goto_documentation" }

(I don't like plugins automatically adding keybinds, okay.)

## Installing

First, you need to have `git` installed and in your `$PATH`. Afterwards you may need to restart Sublime Text 2 before the plugin will work.

### OSX

    $ cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages/
    $ git clone git://github.com/kemayo/sublime-text-2-goto-documentation.git GotoDocumentation

### Linux (Ubuntu like distros)

    $ cd ~/.config/sublime-text-2/Packages/
    $ git clone git://github.com/kemayo/sublime-text-2-goto-documentation.git GotoDocumentation

### Windows 7:

    Copy the directory to: "C:\Users\<username>\AppData\Roaming\Sublime Text 2\Packages"

### Windows XP:

    Copy the directory to: "C:\Documents and Settings\<username>\Application Data\Sublime Text 2\Packages"
