Dice Roller

Grammar

Statment -> ArrayStatement
Statment -> RollStatement

ArrayStatement -> create array Number { RollSequence } DropStatement

RollSequence -> RollSequence RollStatement
RollSequence ->

RollStatement -> roll Number d Number DropStatement

DropStatement -> drop DropWord

Number -> *a number*

DropWord -> lowest
DropWord -> lowest Number
DropWord -> highest
DropWord -> highest Number
DropWord -> random Number
DropWord -> [ Range ]

Range -> ( Number - Number )
Range -> Range Number
Range ->
