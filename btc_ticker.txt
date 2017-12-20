on format_string(this_text, search_string, replacement_string)
	if this_text contains the search_string then
		set AppleScript's text item delimiters to the search_string
		set the item_list to every text item of this_text
		set AppleScript's text item delimiters to the replacement_string
		set this_text to the item_list as string
		set AppleScript's text item delimiters to ""
	end if
	return this_text
end format_string

set stockValue to do shell script "curl -s 'https://api.coinmarketcap.com/v1/ticker/bitcoin/' | grep 'price_usd'"
set stockValue to format_string(stockValue, "        \"price_usd\": \"", "")
set stockValue to format_string(stockValue, "\",", "")
return "" & "$" & stockValue
