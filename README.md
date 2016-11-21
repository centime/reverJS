# reverJS - the Reverse Javascript Constructor

Wrap your javascript code into a ~palindrome !

## Example

Live examples at [http://centime.org/reverJS](http://centime.org/reverJS)

~palindrome for ``alert('reverJS')``:

```js      
/*****************************************************************/
/*                http://centime.org/reverJS                     */
/*     Reverse                                   */([[[0]["reverse"
/*     Javascript                            */]][0+!!+"javascript"
/*     Constructor                           */+!!+0]["constructor"
/*               */]][0](["reverJS"],["return"][0+!!+"~palindromes"
+!!+0]+"  (_=>"+[[]+!+[]][0][3]+"val"+"(reverJS))"))(`
alert('reverJS')                `,`                ('SJrever')trela
`)(("((SJrever)"+"lav"+[3][0][[]+!+[]]+"<=_)  "+[0+!!+
"semordnilap~"+!!+0]["nruter"],["SJrever"])[0][[/*               */
"rotcurtsnoc"][0+!!+/*                           rotcurtsnoC     */
"tpircsavaj"+!!+0][[/*                            tpircsavaJ     */
"esrever"][0]]])/*                                   esreveR     */
/*                     SJrever/gro.emitnec//:ptth                */
/*****************************************************************/
```



## Wrap your javascript code into a ~palindrome

It *doesn't rely on any comments trickery*, everything is about strings and arrays and crazy js behaviors !

* Disclaimer: *a ~palindrome is not a real palindrome*.

    alert([1]) :
    palindromic reverse: )]1[(trela
    ~palindromic reverse: ([1])trela

Special characters which have a symmetrical counterpart are using said counterpart to achieve symmetry. Such characters are: *()[]{}\/<>*

* Warning: *might not be suited for production*.

## Why?

Who doesn't like palindromes ?

## How?

The idea will be to wrap the input into some code that evaluates it, but can be put before as well as after it without raising exceptions. We will use a lot of *strings that are effectively ignored*. Such as in: *eval("INPUT_CODE","EDOC_TUPNI")*.

```js
// using silent parameters in eval:
eval("INPUT_CODE","EDOC_TUPNI")

// using Function to create an "eval" function:
Function(["var1"],"return (_=>eval(var1))")("INPUT_CODE","EDOC_TUPNI")()
```

"Function" can be accessed with *[]["reverse"]["constructor"]*, but the reverse (*["rotcurtsnoc"]["esrever"][]*) is invalid syntax.

Fortunately, we can rewrite it like this: *[[0]["reverse"]][0]["constructor"]*, which reverse, *["rotcurtsnoc"][0][["esrever"][0]]*, quietly returns undefined.

Thus, the following is symmetrical and allows us to execute some code:

```js
(
([[0]["reverse"]][0]["constructor"])
  ("INPUT_CODE")
(["rotcurtsnoc"][0][["esrever"][0]])
)
```

We will use this to return a closure that can be called with meaningless arguments, to execute INPUT_CODE:

```js
(
    (Function(["var1"],"return (_=>eval(var1))"))
        ('INPUT_CODE',"EDOC_TUPNI")
    (("whatever",["whatever"])[undefined])
)
```

When we put all of this together:

```js
(
    ([[[0]["reverse"]][0]["constructor"]][0](
      ["reverJS"],"return (_=>eval(reverJS))"
    ))
        ('INPUT_CODE',"EDOC_TUPNI")
    ((
      "((SJrever)lave>=_) nruter",["SJrever"]
    )[0][["rotcurtsnoc"][0][["esrever"][0]]])
)
```

Adding some complexity just because we can:

```js
(
    ([[[0]["reverse"]][0+!!+"javascript"+!!+0]["constructor"]][0](
        ["reverJS"],["return"][0+!!+"~palindromes"+!!+0]
        +"(_=>"+[[]+!+[]][0][3]+"val"+"(reverJS))")
    )
        ('INPUT_CODE',"EDOC_TUPNI")
    (
        ("((SJrever)"+"lav"+[3][0][[]+!+[]]+">=_)"+
        [0+!!+"semordnilap~"+!!+0]["nruter"],["SJrever"]
    )[0][["rotcurtsnoc"][0+!!+"tpircsavaj"+!!+0][["esrever"][0]]])
)
```

Now that the wrapper is working, all there is left to do is to prepare INPUT_CODE, as a string, to go into our eval function. Since we're using multi-lines strings declared with `, we want to escape this character. But *we need both the original and the symmetric to be escaped*, so \`, which reverse is `/, won't do it.

The trick I used rely on the inline expressions you can put in template literals. *`${'`/'[0]}`* returns '`', and the reverse *`{[0]'\`'}$`* makes the inner ` harmless.

Since the above solution could break in situations The trick I used rely on the inline expressions you can put in template literals. *`${'`/'[0]}`* returns '`', and the reverse *`{[0]'\`'}$`* makes the inner ` harmless.

```js
(/`/g,"${['\`/'][0][0]}")
```

## Links

[http://centime.org/reverJS](http://centime.org/reverJS)
*ping me: /u/centime, quelques.centimes@gmail.com
You might also like [jsf$ck](http://centime.org/jsfsck)
Style shamelessly taken from [JSFuck](http://jsfuck.com)

