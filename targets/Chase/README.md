<h1 align="center">Chase</h1>

```mermaid
graph LR
COMPANY_NAME{Chase}
COMPANY_NAME ---> U{Users} ---> UN[3]
COMPANY_NAME ---> R{Repositories} ---> RN[4]
COMPANY_NAME ---> G{Gists} ---> GN[0]
COMPANY_NAME ---> ML{Most Used<br>Languages}
ML --> Jupyter Notebook
ML --> Go
```