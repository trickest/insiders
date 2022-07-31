<h1 align="center">Monolith</h1>

```mermaid
graph LR
COMPANY_NAME{Monolith}
COMPANY_NAME ---> U{Users} ---> UN[16]
COMPANY_NAME ---> R{Repositories} ---> RN[48]
COMPANY_NAME ---> G{Gists} ---> GN[3]
COMPANY_NAME ---> ML{Most Used<br>Languages}
ML --> JavaScript[JavaScript]
ML --> Python[Python]
ML --> HTML[HTML]
ML --> TypeScript[TypeScript]
ML --> R[R]
```
