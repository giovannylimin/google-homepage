# google-homepage
This is my first project for [The Odin Project](https://www.theodinproject.com) Web Development 101.
The aim is to build the [Google.com](https://www.google.com) homepage.

Here's my project's appearance for the [easy version](https://giovannylimin.github.io/google-homepage/easy-version/)
and here's for the [difficult version](https://giovannylimin.github.io/google-homepage/difficult-version/)

Anyway, this project is made in my corona quarantine, so I used the medical staff image for the profile picture and if you hover over it, it will show a message!

===============================================

My experience while doing this project:

*Easy version*

I used CSS flex for the header and footer.

I had difficulties with creating buttons (mic button and clear input field button) inside the input field, I then used the negative margin value instead to make it seems like it's inside the input field.

I styled the reset button to make it look like the common cancel icon (X) by setting its value attribute `value=""` and give it background image.

The reset button only appears when the input value is focused, i managed to do it with the adjacent sibling selector `input:focus + input[type="reset"`. However, I noticed that the reset button can't do its work. I think it's because when the reset button was clicked, the input field will not in the focused mode, so the reset button will immediately hidden. So I gave `transition-duration: 0.1s;` to give it a little time to process the reset function.

edit: I realized that those buttons inside the searchbar messed up in different browsers, so I changed to `position:absolute` instead (with a proper-positioned container).

I created tooltip when hovering over the mic button.

I removed the default input outline (blue highlight) in the searchbar and styled it with `shadow-box` instead when the field is on hover as well as focused.

I down-sized the images used in icons to make it load faster.

*Difficult Version*

I set the `min-width: 900px;` for `<html>`, and positioned the elements from the left, the only thing that floats to the right is the profile picture.

I reused the code in the easy version for the header and footer part, with extra adjustments. 

I tried to make my form in the searchbar to redirect to another page by using the `action` attribute, however my link is broken because it always shows the privacy error, but if I typed it manually, it shows no problem.

I just realized that I made typo to the link:
`https://www.giovannylimin.github.io/`
I typed the extra `www` which is incorrect.
What it should be:
`https://giovannylimin.github.io/`