# VulnerableWebApp
Este projeto tem por objetivo o desenvolvimento de uma aplicação web intencionalmente vulnerável.

## Aviso Legal
As vulnerabilidades e não conformidades aqui presentes foram propositalmente colocadas para fins educacionais apenas. Em hipótese alguma incentivamos o uso de tais más práticas.

## Pré-requisitos
* Tenha ambos servidores Apache e MySQL instalados e configurados. Confira <a href="#tecnologias-utilizadas">Tecnologias Utilizadas</a> para mais detalhes.
* Dê permissão de escrita ao diretório `uploads` no servidor da aplicação, para que os arquivos possam ser transferidos ao diretório durante o processo de *upload*.

## Sobre a Aplicação
Trata-se de um fórum em que os usuários podem compartilhar mensagens entre si através de suas postagens.
* O usuário pode cadastrar, editar e excluir sua conta, além de cadastrar, editar e excluir suas próprias postagens.
* O administrador pode, além das funções já existentes de um usuário comum (com exceção de excluir sua conta), pode excluir as postagens dos demais usuários e suas contas.

### Vulnerabilidades e não conformidades intencionalmente colocadas
* Fraca política de senhas (ou falta dela);
* Tratamento de erro inapropriado;
* *Brute-force Attack;*
* *XSS (Cross-Site Scripting)*
  * *Reflected;*
  * *Stored;*
* *SQL Injection*
  * *In-band;*
  * *Inferential;*
* *Unrestricted File Upload;*
* *File Inclusion*
  * *LFI;*
  * *RFI;*
* *Command Execution.*

Lembrando que podem haver mais vulnerabilidades do que as listadas acima.

## Tecnologias Utilizadas
* HTML5 e CSS3
* PHP versão 7.2.24
* Apache versão 2.4.29
* MySQL versão 5.7.27

## Regras de Diretórios
* Diretórios de desenvolvimento devem estar no modelo MVC.
* Arquivos extras do Front-end devem ficar no diretório `modules`.
* A documentação deve ficar no diretório `docs`.

## Diretórios
```sh
|-- controller
|-- docs
|-- model
|-- modules
|-- persistence
|-- uploads
|-- view
```