# Programming a Guessing Game

```cpc
txt/ Guess the number!
fix/ number = /F:CPC.INT(%CPC.RND%)

:loop:

txt/ Please input your guess.
fix/ /q guess
txt/ You guessed: %guess%

if/ "%guess%" == "%number%" then:
    txt/ You win!
    stop/
else:
    if/ "%guess%" > "%number%" then:
        txt/ Too big!
    else:
        txt/ Too small!
    end/ if
end/ if

goto/ loop
```