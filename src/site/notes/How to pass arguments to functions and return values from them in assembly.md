---
{"dg-publish":true,"permalink":"/how-to-pass-arguments-to-functions-and-return-values-from-them-in-assembly/","tags":["datorteknik"]}
---


Where do we store the temporary values of a function without overwriting existing data in registers? We put it in the [[Stack\|stack]]. The [[Stack\|stack]] contains the address to return to. After the function is done we clear our temporary variables from the [[Stack\|stack]], which reveals the return address. 

If we want to use the [[Register\|register]] we have to push it's value to the [[Stack\|stack]] and then make sure to pop the [[Stack\|stack]] in the right order so we get the value back at the end of the function (and put it back in the [[Register\|register]]).

*Register Usage Convention* some registers are "call-saved" and other "call-used", with different rules for usage.