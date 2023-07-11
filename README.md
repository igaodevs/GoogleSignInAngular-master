Este repositório é um exemplo de como usar o Google Identity Sign In com Angular, diretamente, sem usar nenhuma biblioteca externa.

Você deve considerar usar o Google Identity Library diretamente porque:

1) A plataforma da biblioteca JavaScript do Google está obsoleta e deixará de ser utilizada a partir de março de 2023.

2) No momento, a biblioteca externa para login do Google (angularx-social-login) também está obsoleta por causa disso.

3) Se o angularx-social-login for atualizado para o Google Identity, será apenas para o Angular 13 e versões posteriores. Portanto, se você tiver uma versão anterior, esta pode ser uma solução para você.

# O que fazer:

1) Adicione a tag de script do Google Identity, conforme mostrado no arquivo index.html.
2) Adicione uma div com um ID, conforme mostrado no arquivo app.component.html.
3) Siga as alterações no arquivo app.component.ts.
4) Certifique-se de colocar o seu próprio ID do cliente do Google em seu devido lugar, no arquivo app.component.ts.

*Última observação, para desenvolvimento local, certifique-se de mencionar tanto http://localhost quanto http://localhost:4200 nas "Origens Javascript Autorizadas" da plataforma de nuvem do Google.

# Angular 13

Este projeto foi gerado com o [Angular CLI](https://github.com/angular/angular-cli) versão 13.3.7.

## Servidor de desenvolvimento

Execute `ng serve` para iniciar um servidor de desenvolvimento. Acesse `http://localhost:4200/`. O aplicativo será recarregado automaticamente se você alterar qualquer um dos arquivos de origem.

## Scaffolding de código

Execute `ng generate component nome-do-componente` para gerar um novo componente. Você também pode usar `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Execute `ng build` para compilar o projeto. Os artefatos de compilação serão armazenados no diretório `dist/`.

## Executando testes unitários

Execute `ng test` para executar os testes unitários via [Karma](https://karma-runner.github.io).

## Executando testes de ponta a ponta

Execute `ng e2e` para executar os testes de ponta a ponta usando uma plataforma de sua escolha. Para usar este comando, você precisa primeiro adicionar um pacote que implemente recursos de teste de ponta a ponta.

## Ajuda adicional

Para obter mais ajuda sobre o Angular CLI, use `ng help` ou consulte a página [Angular CLI Overview and Command Reference](https://angular.io/cli).
