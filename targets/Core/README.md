<h1 align="center">Core</h1>

```mermaid
graph LR
COMPANY_NAME{Core}
COMPANY_NAME ---> U{Users} ---> UN[2]
COMPANY_NAME ---> R{Repositories} ---> RN[4]
COMPANY_NAME ---> G{Gists} ---> GN[4]
COMPANY_NAME ---> ML{Most Used<br>Languages}
ML --> Vim_Script[Vim Script]
ML --> TeX[TeX]
ML --> Python[Python]
ML --> Java[Java]
```
