# Run the app
`bundle install`
`rails serve`
*Make sure selenium is running to avoid sanitize error*  

a) How you would generate a unique ID for each URL
For each url I used a formula **rand(36*8).to_s(36)** to generate a unique key to associate with the long url  

b) How you would generate unique IDs at scale (8K+ requests per second)
The current implimentation uses microservices  
c) How your service would handle redirects
redirects are handled directly in the code  

d) How you would support custom short URLs
Currently not implemented 
but this would require me to use the custom address(https://t.co) and use a DNS lookup to pass the id(Efg5464D)  

e) How you would delete expired URLs
The system would require the a default expiry timer this can also be specified by the user, this would allow for the system to run a cron job and clean up the server   

f) How you would track click stats
store the number of times the url is referenced  
g) Draw flowcharts diagrams and architecture diagram for this service.  

