# unexpected-token.  (syntax error)

When Javascript engine can't parse the file because I made an error in my code. It canot make it past the creationphase.

More specifically, I started something I didn't finish. Opened paranthesis I never closed, used an operator with no operand.

I first came across this error studying type coercion when I tried to typeof the void operator.

I expect this error will be a real pain because the message isn't very helpful. It tells me there's something missing, but always.
I'll have to go back to reading my WHOLE FILE to find where I made my mistake.

___

£ Code where I first found the error

```Javascript
typeof void

// comments
```

```Javascript
typeof void;

// comments
```


These look so similar, but are soooo different. With the semicolo JS catches the error before moving on to the rest of the file. This way it tells me if there is an error on Line 1 itself and not go all the way to the end yet give me an unhelpful error.
