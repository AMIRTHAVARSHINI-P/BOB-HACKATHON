# BOB-HACKATHON
ones[ ] ← {”One”, ”T wo”, ”T hree”, ...”N ineteen”}
 tens[ ] ← {”T wenty”, ”T hirty”, ”F orty”, ...”N inety”}
 S ← null
 output ← null

 Function convert(number):
 if number > 19 then
 if number%10 = 0 then
 S = tens[(number/10) − 1]
 else
 S = tens[(number/10) − 1] + ” ” + ones[number%10]
 else
 S = ones[number]
 end
 return S
 End Function

 Function num2words(number):
if len(number) > 7 then
output ← output + crore
 if len(number) > 5 then
 output ← output + lakh
 if len(number) > 3 then
 output ← output + thousand
 if len(number) > 2 then
 output ← output + hundred
 if number > 100 and (number%100) then
 output ← output + ”and”
output ← output + convert(number%102
)
 if len(number) = 2 and (number > 19) then
 output ← convert(number)
 if (len(number) = 2 and number ≤ 19) or (len(number) = 1) then
 output ← ones[number − 1]
 return output
End Function

Function compare(string 1, string 2):
if string 1 = string 2 then
Result ← ”Matching”
else
 Result ← ”N ot Matching”
 end
return Result
 End Function

 crore ← output + convert(number/107
) + ”Crore”
 lakh ← output + convert((number/105

)%100) + ”Lakh”
 thousand ← output + convert((number/103

)%100) + ”T housand”

 hundred ← output + convert((number/102

)%10) + ”Hundred”


// Courtesy amount to words
 courtesy in words ← num2words(number)

// Comparing Courtesy amount in words with Legal Amount
 result ← compare(courtesy in words, legal amount)
