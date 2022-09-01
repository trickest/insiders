<h1 align="center">Monolith</h1>

```mermaid
graph LR
COMPANY_NAME{Monolith}
COMPANY_NAME ---> U{Users} ---> UN[10]
COMPANY_NAME ---> R{Repositories} ---> RN[80]
COMPANY_NAME ---> G{Gists} ---> GN[19]
COMPANY_NAME ---> ML{Most Used<br>Languages}
ML --> Python[Python]
ML --> MATLAB[MATLAB]
ML --> JavaScript[JavaScript]
ML --> PHP[PHP]
ML --> C#[C#]
```
