Backup Schema
![[Pasted image 20250711161159.png]]
![[Pasted image 20250711161208.png]]
![[Pasted image 20250711161217.png]]
![[Pasted image 20250711161229.png]]
![[Pasted image 20250711161237.png]]
![[Pasted image 20250711161243.png]]
## Edit File SQL File


```
CREATE DATABASE masterdata_db WITH TEMPLATE = template0 ENCODING = 'UTF8' LOCALE_PROVIDER = libc LOCALE = 'en_US.utf8';

\connect masterdata_db
```


Remove

- \connect masterdata_db
- LOCALE_PROVIDER = libc LOCALE = 'en_US.utf8'