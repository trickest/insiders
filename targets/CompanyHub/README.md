<h1 align="center">CompanyHub</h1>

```mermaid
graph LR
COMPANY_NAME{CompanyHub}
COMPANY_NAME ---> U{Users} ---> UN[1]
COMPANY_NAME ---> R{Repositories} ---> RN[6]
COMPANY_NAME ---> G{Gists} ---> GN[1]
COMPANY_NAME ---> ML{Most Used<br>Languages}
ML --> C++[C++]
ML --> Java[Java]
ML --> C[C]
```
