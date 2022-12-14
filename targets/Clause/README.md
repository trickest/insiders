<h1 align="center">Clause</h1>

```mermaid
graph LR
COMPANY_NAME{Clause}
COMPANY_NAME ---> U{Users} ---> UN[6]
COMPANY_NAME ---> R{Repositories} ---> RN[65]
COMPANY_NAME ---> G{Gists} ---> GN[15]
COMPANY_NAME ---> ML{Most Used<br>Languages}
ML --> Shell[Shell]
ML --> Rust[Rust]
ML --> Nix[Nix]
ML --> Vim_Script[Vim Script]
ML --> Dockerfile[Dockerfile]
```
