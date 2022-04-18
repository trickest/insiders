<h1 align="center">Monolith</h1>

```mermaid
graph LR
COMPANY_NAME{Monolith}
COMPANY_NAME ---> U{Users} ---> UN[8]
COMPANY_NAME ---> R{Repositories} ---> RN[36]
COMPANY_NAME ---> G{Gists} ---> GN[8]
COMPANY_NAME ---> ML{Most Used<br>Languages}
ML --> JavaScript[JavaScript]
ML --> Ruby[Ruby]
ML --> C#[C#]
ML --> TypeScript[TypeScript]
ML --> Python[Python]
```
