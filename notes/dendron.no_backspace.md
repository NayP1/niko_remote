---
id: j9a5yd64gojlj9akw1p7ef1
title: No_backspace
desc: ''
updated: 1676908545380
created: 1676908375793
---
In Markdown you cannot add simple backspaces to add space.

If the markdown text is converted to HTML and rendered in browsers, then you can use the following technique to add multiple spaces between texts.

Solution : Use ```&nbsp``` : (Non-Breaking Space)

### A bonus time-saving trick
Only multiple space characters() are converted to a single space character, so you can combine the space character with ```&nbsp```;. So if you want, say, 6 spaces, you could combine 6 space characters with ```&nbsp```;.

Ex : I have 6 spaces before &nbsp; &nbsp; &nbsp;me
