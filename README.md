# reverJS
the Reverse Javascript Constructor

Generating near-palindrome, symmetric javascript code.

This is a work in progress, more to come soon.

##Example

```js      
/*****************************************************************/
/*                http://centime.org/reverJS                    */
/*     Reverse                                   */([[[0]["reverse"
/*     Javascript                            */]][0+!!+"javascript"
/*     Constructor                           */+!!+0]["constructor"
/*               */]][0](["reverJS"],["return"][0+!!+"~palindromes"
+!!+0]+"  (SJrever=>"+[[]+!+[]][0][3]+"val"+"(reverJS))"))(`\ /**\/
                  alert('Reverse Javascript '+
             'Constructor')`+'\ /*\ /'+`('rotcurtsnoC'             
                     +' tpircsavaJ esreveR')trela                  
\ /**\/`)(("((SJrever)"+"lav"+[3][0][[]+!+[]]+"<=reverJS)  "+[0+!!+
"semordnilap~"+!!+0]["nruter"],["SJrever"])[0][[/*               */
"rotcurtsnoc"][0+!!+/*                           rotcurtsnoC     */
"tpircsavaj"+!!+0][[/*                            tpircsavaJ     */
"esrever"][0]]])/*                                   esreveR     */
/*                    SJrever/gro.emitnec//:ptth                */
/*****************************************************************/
```

## Notes

* Creates ~palindromes, not real palindromes:

  * palindrome: `alert(1)` -> `')]1[(trela'`

  * ~palindrome: `alert(1)` -> `'([1])trela'`

* "reverJS" and "SJrever" are defined in the context the code is ran in. But can be rewritten safely.

## Caveats

    // Breaks:
    //   -run
          // }}$$
          // }*$
    //       lastline = //comment
    //   -symmetry
    //       `
  

## Explanations

Symmetric eval:

```js
// Structure
(
	(Function)(["var1"],"return (var2=>eval(var1))")
		('console.log(1)')
	("whatever"||undefined)
)
// Solution
(
	([[[0]["reverse"]][0]["constructor"]][0](["reverJS"],"return (SJrever=>eval(reverJS))"))
		("console.log(1)")
	(("((SJrever)lave>=reverJS) nruter",["SJrever"])[0][["rotcurtsnoc"][0][["esrever"][0]]])
)
// with some styling:
(
	([[[0]["reverse"]][0+!!+"javascript"+!!+0]["constructor"]][0](
		["reverJS"],
		["return"][0+!!+"~palindromes"+!!+0]
		+" (SJrever=>"+[[]+!+[]][0][3]+"val"+"(reverJS))")
	)
		("console.log(1)")
	(
		("((SJrever)"+"lav"+[3][0][[]+!+[]]+">=reverJS) "+
		[0+!!+"semordnilap~"+!!+0]["nruter"]
		,["SJrever"]
	)[0][["rotcurtsnoc"][0+!!+"tpircsavaj"+!!+0][["esrever"][0]]])
)
```


Symmetric expression:

```js
/**/console.log(1)/*/(1)gol.elosnoc/**/
```


Symmetric escaping:

```js

```