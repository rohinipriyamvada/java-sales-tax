# TAX

on Normal goods -> 10%
Exceptions: food, books, medical products

on imported goods -> 5%
Exceptions: null

Rounding of tax -> 
rate = n% 
price = p

tax(round) = np/100

* The inputs are categorised into imported and non-imported
* Imported (no exceptions) calculate tax 
* Add tax and finalise
* Have a list of categories of items, one item in each category (food, books, medical prods)
* Then for non-imported if it belongs to exceptional category don't add tax and finalse the price
* If not calculate the tax
* Add tax to the price
* add all the final prices 
* add all the tax amount
* Display!!!

## Classes
importedGoodsTax(array of goods with details)
* each item set if maps{<Name>, <price>, <tax>}
* all items list of sets [{}, {}]

localGoodsTax(array of goods with details)
* each item set if maps{<Name>, <price>, <tax>}
* all items list of sets [{}, {}]
* if (inCategories) => calculateTax
* return price and tax as 00.00

calculateTax(price, rate)
* return set of maps <new price> and <tax amount>

finalPrices(all items list of sets [{}, {}])
* Add all the taxes
* Add all the prices
* sout it!