ke IP address se link karna. Yeh kaam aap Route 53 ya kisi bhi DNS provider ke through kar sakte ho.
Agar aapka domain AWS Route 53 mein hai:

    Login to AWS jhjhjnknknm,e.

    Open Route 53 service.

    name nishant hai

    Create Record par click karo.

    Record banate waqt:

        Record name: (khaali chhodo agar root domain hai, ya www agar subdomain chahiye)

        Record type: A – IPv4 address

        Value: Apna EC2 instance ya load balancer ka IP address

        Routing policy: Simple

        TTL (Time to live): Default chhodo ya apni marzi ka set karo

        Save record

Agar aapka domain kisi aur provider jaise GoDaddy, Namecheap mein hai:

    Apne DNS provider ke dashboard mein login karo.

    Domain ke DNS Management section mein jao.

    A record add karo:

        Host: @ (for root domain) ya www (for subdomain)

        Points to: AWS ka public IP address

        TTL: Default rehne do

    Save karo.

EC2 ke liye caution:

    Agar aap Elastic IP use nahi karte ho to EC2 ka public IP restart ke baad change ho jata hai.

    
dvchb cmdsc nc  c cdscc 
cnsdnvdvvnvm,czv v n,xzc
ncnc cmc cm 