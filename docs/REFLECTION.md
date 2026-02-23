# Reflection

Answer each question in 2-3 sentences.

## Most surprising discovery

Which vulnerability surprised you the most to find? Why didn't you expect it?

The most surprising vulnerability was the secret remaining in git history. I initially thought removing it from the source code was enough, but I learned that secrets persist in past commits unless history is rewritten. That highlighted how important version control is for security. 

## Real-world risk

Pick one vulnerability you found. How would you explain its danger to a teammate who's never heard of it?

The XSS vulnerability could allow an attacker to inject scripts into the page through user input. In a real application, this could lead to data theft, or unauthorized actions performed on behalf of other users which would be horrible. 

## Future practice

What specific habit or check will you add to your own coding workflow to catch these issues before they ship?

Going forward, I will avoid committing secrets by using environment variables from the start. I will also run dependency audits regularly and be more cautious about rendering user input directly. 