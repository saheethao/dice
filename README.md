# Dice Roller
## Grammar 1
<pre>
Statement -> Roll Drop

Roll      -> Result Op Result

Result    -> Roll
Result    -> Dice
Result    -> Number

Dice     -> Number d Number

Number   -> INT

Drop     -> lowest
Drop     -> lowest Number
Drop     -> highest
Drop     -> highest Number
Drop     -> random Number
Drop     -> [ Range ]

Range    -> ( Number - Number )
Range    -> Range Number
Range    ->
</pre>
## Grammar 2
<br/><br/>
Statment -> ArrayStatement<br/>
Statment -> RollStatement
<br/><br/>
ArrayStatement -> create array Number { RollSequence } DropStatement
<br/><br/>
RollSequence -> RollSequence RollStatement<br/>
RollSequence ->
<br/><br/>
RollStatement -> roll Number d Number DropStatement
<br/><br/>
DropStatement -> drop DropWord
<br/><br/>
Number -> *a number*
<br/><br/>
DropWord -> lowest<br/>
DropWord -> lowest Number<br/>
DropWord -> highest<br/>
DropWord -> highest Number<br/>
DropWord -> random Number<br/>
DropWord -> [ Range ]<br/>
<br/><br/>
Range -> ( Number - Number )<br/>
Range -> Range Number<br/>
Range -><br/>
