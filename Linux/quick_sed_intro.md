## SHORT INTRO TO ``sed``
*Me*:   wat did u teach me abt `sed` yesterday 

*GPT*:  Yesterday, I taught you about the `sed` command, which is a powerful text editor that can perform find and replace operations on text files.

Here is a brief summary of what we covered:

`sed` stands for "stream editor", and is used to modify text files by performing search and replace operations on them. The basic syntax of the `sed` command is

```console
sed 's/sadness/happiness/g' input_file > output_file
``` 

where:  
- `old_text` is the string you want to replace  
- `new_text` is the replacement string  
- `g` is the "global" flag that replaces all occurrences of the string  
- `input_file` is the file you want to edit,  
- and `output_file` is the file where the edited text will be saved.  
> Note: the `/` acts as a separator with sed, just as [`space`] acts as a separator in bash. **You can use any character you want as a separator, as long as it is not used in the strings you are searching for or replacing.**

You can use `sed` to edit a file in place, without creating a new file, by using the -i option, like this:
```console
sed -i 's/sadness/happiness/g' input_file
```
You can use regular expressions in `sed` to perform more complex search and replace operations, such as replacing a string only if it appears at the beginning of a line, or replacing a string only if it is surrounded by certain characters.

You can also use `sed` to delete lines from a file, using the `d` command, 

or to insert or append text to a file, using the `i` or `a` commands. 

Overall, `sed` is a powerful tool for editing text files, and can save you a lot of time and effort when making changes to large or complex files.
Read more about `sed` here:
- [My follow up article 🙂](https://angel.hashnode.dev/short-sed-intro)
- [Sed - An Introduction and Tutorial by Bruce Barnett](https://www.grymoire.com/Unix/Sed.html)
- [sed-documentation](https://www.gnu.org/software/sed/manual/sed.html#Introduction) 
