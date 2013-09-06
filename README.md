# Page Title Shortener

[Greasemonkey][greasemonkey] script that shortens a webpage's title based on user-defined rules. Useful for sites such as wikis that have long titles.

[greasemonkey]: https://github.com/greasemonkey/greasemonkey/ 

## Installation

Usage instructions are posted below and can also be found in the script source.

After installation, follow these steps:  
1. Go to Firefox's about:config page (type "`about:config`" into the address bar).  
2. Right-click anywhere and choose the menu option to create a new string.  
3. Give the preference name `"extensions.greasemonkey.scriptvals.PageTitleShortener/Page Title Shortener.data"`  
4. Set the value to the rules you want. Use the data format below. See the example or refer to the [JSON home page][json] for more help.  
5. Add the website URL regex to the list of included pages via the Greasemonkey add-on page options. This list must be kept in sync with changes you make to the data preference variable.

[json]: http://www.json.org/

## Data Format

JSON array format with field values as follows:

* index 0 = wesite URL match (*regex*)
* index 1 = text want to replace (*regex*)
* index 2 = text to replace with (*plaintext*)

### Example

    extensions.greasemonkey.scriptvals.PageTitleRewriter/Page Title Shortener.data = 
        [["darksoulswiki.wikispaces.com", "Dark Souls Wiki -", "DS: "]]

## Homepage

[View on userscripts.org](http://userscripts.org/scripts/show/154851)
