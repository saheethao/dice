# Dice Roller
## Grammar 1

Statement -> Roll Drop<br/>
<br/><br/>

Roll      -> Result Op Result<br/>
<br/><br/>

Result    -> Roll<br/>
Result    -> Dice<br/>
Result    -> Number<br/>
<br/><br/>

Dice -> Number d Number<br/>
<br/><br/>

Number -> INT<br/>
<br/><br/>

Drop     -> lowest<br/>
Drop     -> lowest Number<br/>
Drop     -> highest<br/>
Drop     -> highest Number<br/>
Drop     -> random Number<br/>
Drop     -> [ Range ]<br/>
<br/><br/>

Range    -> ( Number - Number )<br/>
Range    -> Range Number<br/>
Range    -><br/>
<br/><br/>

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
