

Markdown Support
LaRecipe automatically leverages Markdown to HTML parser out of the box.

Basics
Tables
Alarms
Table of Content

Basics
Markdown elements automatically parsed into normal HTML tags.

TYPOGRAPHY
Input:

###### H6
Output:

H6


IMAGES
Input:

![image](url)
Output:

cute image



INLINE CODE
Input:

Inline code is `cool`
Output:

Inline code is cool



CODE
LaRecipe uses prism.js with code highlighting out of the box. Currently supported languages: [php, js, text, c, c++, html, text]

Input:

```php 
echo 'LaRecipe is beatiful'; 
```

Output:

echo 'LaRecipe is beatiful';

Tables
Markdown Tables automatically parsed and converted to nice looking rendered tables. Thanks to Argon and CSS :D

Input:

| # | Name   | Age |
| : |   :-   |  :  |
| 1 | Saleem | 24  |
| 2 | John   | 25  |
| 3 | Ayman  | 26  |
Output:

#	Name	Age
1	Saleem	24
2	John	25
3	Ayman	26

Alarms
LaRecipe provides beautiful looking alerts parsed directly from Markdown with extra sugar, all that you have to do is to prepend Markdown blockquote with {type} of your alert.

The supported alarms types are: primary, success, info, danger, warning.

Input:

> {danger} Here is an example of danger alarm message
Output:

Here is an example of danger colored alarm


Table of Content
By default, LaRecpie is considering the first ul element in your docs file as the table of content and it will appear on the top-right corner of your documentation for quick navigation.

Each link in your table of content will be targeted to the corresponding h2 element in your documentation file.

- [Example](#example-link)

<a name="example-link">
## Example
