<h1 align="center">UrbanCompany</h1>

```mermaid
graph LR
COMPANY_NAME{UrbanCompany}
COMPANY_NAME ---> U{Users} ---> UN[5]
COMPANY_NAME ---> R{Repositories} ---> RN[50]
COMPANY_NAME ---> G{Gists} ---> GN[0]
COMPANY_NAME ---> ML{Most Used<br>Languages}
ML --> JavaScript[JavaScript]
ML --> HTML[HTML]
ML --> PHP[PHP]
ML --> CSS[CSS]
ML --> Jupyter_Notebook[Jupyter Notebook]
```