# ZZCMS2021 

Location
----
    http://www.zzcms2021.com/index.php

Affected Products
----
    ZZCMS2021
Poc
----
    1.Set up ZZCMS and access the default page normally: http://www.zzcms2021.com/index.php

    2.Construct three HTM files containing malicious code named "bottom.htm", "index.htm", "top_index.htm". And then somehow upload it to the server on any path. For example, you can upload malicious files to the wordpress path through a CMS such as wordpress. Of course, you can upload anywhere on the server in some way, but not anywhere in the Apache directory.
    
    3.Intercept current access information with Burpsuite, modify request lines, and add parameters “skin=../../wordpress0581”,then continue to submit.
    
    4.At this point, you can see that "Success" pops up on the page, and click OK to pop up the user's cookie information saved in the current directory.
