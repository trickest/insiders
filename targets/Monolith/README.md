<h1 align="center">Monolith</h1>

```mermaid
graph LR
COMPANY_NAME{Monolith}
COMPANY_NAME ---> U{Users} ---> UN[16]
COMPANY_NAME ---> R{Repositories} ---> RN[74]
COMPANY_NAME ---> G{Gists} ---> GN[11]
COMPANY_NAME ---> ML{Most Used<br>Languages}
ML --> JavaScript[JavaScript]
ML --> Rust[Rust]
ML --> Python[Python]
ML --> Swift[Swift]
ML --> PHP[PHP]
```
