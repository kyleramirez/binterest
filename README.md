

```ruby
require "open-uri"
require "nokigiri"

doc = Nokogiri::HTML(open("https://www.cardigan.cards/"))
doc.at("meta[name='description']")["content"]
doc.at("meta[property='og:description']")["content"]
```


