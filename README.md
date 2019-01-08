# javascript sessionStorage shopping cart
A complete shopping cart built with Javascript and sessionStorage. Includes PayPal payments.
I wrote this shopping cart script after Gabriele Romanato's tutorial on Smashing Magazine. All credit goes to him for it's design and concepts. His tutorial however, used JQuery. I wanted to rewrite it in vanilla Javascript. You can find his tutorial below:
https://www.smashingmagazine.com/2014/02/create-client-side-shopping-cart

You can see his JQuery version in his repository:
https://github.com/gabrieleromanato/jQuery-sessionStorage-shopping-cart

Gabriele Romanato's tutorial focused on the proof-of-concept of a shopping cart using sessionStorage to store data while retaining the ability to navigate to different pages. It did not focus on form validation. While validation is welcome, trying to cover all the aspects and security risks defeats the purpose of his tutorial.

Now for the fun. Since I am a Javascript advocate and hate using JQuery with every fiber I have, I felt it my mission to rewrite this script for those who also don't use JQuery. It was a troubling task as I have avoided learning JQuery all these years. Furthermore, you have made use of OOP (Object Oriented Programming). A concept which I grasped with PHP but, had yet to use in Javascript. So it was time to bust out my reading glasses. This article, for me, became more of a task to learn OOP in Javascript than it was learning sessionStorage. A feature which I had already learned. That said, you had used OOP and self invoking functions with closures. These self invoking functions eliminated the need for inline script statements in the markup. A concept that triggered a light bulb for me. So thanks for that. Although, I think it would have been helpful to point out that small detail. I am by no means a starter with Javascript. But I am completely self taught, so I never got around to learning self invoking functions and closures. Nor did I have a need for them, until now.

Furthermore, my knowledge of using prototypal scripting was almost none. So I ended up learning a ton about prototypes. Ironically, had I just created my own shopping cart from my head, without the aid of a tutorial, I probably would have not used OOP or self invoking function calls. Nor would I have added prototype objects. So while I cursed spending the time to learn these concepts, I am grateful for the experience. My tool-belt is much larger now.

I wrote this script in vanilla Javascript and I really hope you will give it a look over. Since I wrote it line for line (zero copying and pasting), there are differences. However, I stuck to exact variable names and markup ID's to make it appear the same as the JQuery version, plus it can be used with the same HTML markup that you provided. Now, because Javascript does not have a built in "slide" function, I had to write my own. So that is really the only difference between the two versions. In a couple of areas of the JQuery version, code was redundant, so I simplified. Also I ran into trouble using "this.element". Javascript wants "document." when calling element ID's. So I stuck with that. If there is a better way, please let me know.

Tested on Chrome (version 63.0.3239.132), with Windows 7. No errors so far. Although, I have not really tested the validation function for errors from user input, as this article really isn't about validation. Of course, validation improvements are welcome, but that really defeats the goal of this article.

P.S. Some functions used "var self = this;", some did not. Not sure if that was intention, accident, or laziness. Either way, I added the statement to all functions that used the keyword "this".
