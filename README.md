# MmExchangeRate

A simple exchange rate checker and calculator based on [Central Bank of Myanmar Api](http://forex.cbm.gov.mm/index.php/api) in elixir.

Before you try it, make sure you've install [elixir 1.*](http://elixir-lang.org/install.html)

	$ git clone git@github.com:Arkar-Aung/mmExchangeRate.git
	$ cd mmExchangeRate
	$ mix deps.get
	$ iex -S mix


##### To check available currency list

	MmExchangeRate.currencies()

##### To check today exchange rate

	MmExchangeRate.today("usd") # default currency is usd if paramter is empty

##### To calculate rate with today exchange rate

	MmExchangeRate.calculate(100, "usd") # default currency is usd if paramter is empty

##### To check exchange rate history

	MmExchangeRate.from("dd-mm-yyyy", "usd") # default currency is usd if paramter is empty	

