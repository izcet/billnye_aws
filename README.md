# Bill Nye AWS Test

### THE IDEA:
I don't know AWS, but I do have a domain name that I own that is not currently being used.
I could kill two birds with one stone by deploying my first S3 site and putting content on the domain.
<br><br>

### THE BACKSTORY:
One of my vices is my habit of impulse buying. 
What I buy (from Magic Cards to Domain names) depends on my current addiction, though they're ususally cheap (~99c) and therefore easy to rationalize.
<br><br>
So I bought billnyethe.science with the justification that at some point, _eventually_, I would make a website `billnyethe.science/guy`. You know, for the lulz.
<br><br>
Fast forward six months and I'm still not using it, but I need to teach myself AWS in preparation for an interview.
<br><br>

### THE EXECUTION
Mixed results. Everything here took a little over an hour for me, minus a break for dinner.
<br><br>

### WHAT WORKED
- Inside this repository is the source code for the basic placeholder I would host until I got the site working, after which I would further develop it to be more presentable.
- Starting an S3 instance and uploading the code was painless and easy, if a bit overwhelming at first just because I was navigating a new web portal, but the developer tools and documentation got me along.
<br><br>

### WHAT DIDN'T WORK
- AWS Route 53 prefers you to have the domain name hosted through AWS, not another nameserver.
- AWS Route 53 does not include specialty domain names, you know, like `.science`.
- AWS doesn't provide a static IP, so I can't set up an `A Record` alias through my current nameserver.
<br><br>

### WHAT I COULD DO
I could set up a computer (either Digital Ocean or a physical one) with a static IP address to use as a proxy, that points to my S3 Bucket. This would:
- Have a static IP that my nameserver could attach to
- Route the traffic to the S3 bucket where the site is hosted.

This does however defeat the purpose of having the S3 host the website if I need to have another machine up anyways.
<br><br>

### WHAT I LEARNED
- AWS is pretty easy to get started
- DNS and routing is pretty complicated
- Technicalities are a dumb barrier for progress
