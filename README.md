# Excel_formulas
Round
1. =ROUND(A1, 2)
2. =ROUND(2.15, 1) Rounds 2.15 to one decimal place 2.2

=ROUND(2.149, 1) Rounds 2.149 to one decimal place 2.1

=ROUND(-1.475, 2) Rounds -1.475 to two decimal places -1.48

=ROUND(21.5, -1) Rounds 21.5 to one decimal place to the left of the decimal point 20

=ROUND(626.3,-3) Rounds 626.3 to the nearest multiple of 1000 1000

=ROUND(1.98,-1) Rounds 1.98 to the nearest multiple of 10 0

=ROUND(-50.55,-2) Rounds -50.55 to the nearest multiple of 100 -100

=check value is no and apply function if value is no
=IF(ISERROR(C13/1),"Invalid Data",(B13*C13)/100) 

SUM IF not equal to
To build the "not equal to" criteria, use the "<>" logical operator.

When a value, either text or number, is hardcoded in the criteria, remember to surround the entire construction with double quotes.

For example, to sum the amounts with shipment other than 3 days, the formula goes as follows:

=SUMIF(C2:C10, "<>3", B2:B10)

To find a total of all the items except Apples, the formula is:

=SUMIF(A2:A10, "<>apples", B2:B10)

When the criterion is in another cell, concatenate the "not equal to" operator and a cell reference like this:

=SUMIF(A2:A10, "<>"&F1, B2:B10)
