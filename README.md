# Sobre o arquivo README do repositório

Você pode adicionar um arquivo README ao seu repositório para informar outras pessoas por que seu projeto é útil, o que elas podem fazer com o projeto e como elas podem usá-lo.

## Sobre READMEs

É possível adicionar um arquivo README a um repositório para comunicar informações importantes sobre o seu projeto. Um README, juntamente com uma licença de repositório, um arquivo de citação, diretrizes de contribuição e um código de conduta, comunica as expectativas para seu projeto e ajuda você a gerenciar contribuições.

Para obter mais informações sobre como fornecer diretrizes para seu projeto, consulte [Adicionar um código de conduta ao seu projeto](/pt/communities/setting-up-your-project-for-healthy-contributions/adding-a-code-of-conduct-to-your-project) e [Configurar seu projeto para contribuições saudáveis](/pt/communities/setting-up-your-project-for-healthy-contributions).

Um README, muitas vezes, é o primeiro item que um visitante verá ao visitar seu repositório. Os arquivos README geralmente incluem informações sobre:

* O que o projeto faz
* Por que o projeto é útil
* Como os usuários podem começar a usar o projeto
* Onde os usuários podem obter ajuda com seu projeto
* Quem mantém e contribui com o projeto

Se você colocar o arquivo README no diretório oculto `.github`, raiz ou `docs`, GitHub reconhecerá e exibirá automaticamente o seu README aos visitantes do repositório.

Se um repositório contiver mais de um arquivo README, o arquivo mostrado nos links será escolhido nos locais na seguinte ordem: o diretório `.github`, o diretório raiz do repositório e, por fim, o diretório `docs`.

Quando o README for exibido no GitHub, qualquer conteúdo além de 500 KiB será truncado.

Se você adicionar um arquivo README à raiz de um repositório público com o mesmo nome de usuário, esse README aparecerá automaticamente na sua página de perfil. Você pode editar seu perfil README com GitHub o Flavored Markdown para criar uma seção personalizada em seu perfil. Para saber mais, confira [Gerenciar o README do seu perfil](/pt/account-and-profile/how-tos/profile-customization/managing-your-profile-readme).

## Sumário gerado automaticamente para arquivos markdown

Para a exibição renderizada de qualquer arquivo Markdown em um repositório, incluindo arquivos README, GitHub gerará automaticamente um sumário com base em títulos de seção. Você pode exibir o sumário de um arquivo README clicando no ícone <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-list-unordered" aria-label="Table of Contents" role="img"><path d="M5.75 2.5h8.5a.75.75 0 0 1 0 1.5h-8.5a.75.75 0 0 1 0-1.5Zm0 5h8.5a.75.75 0 0 1 0 1.5h-8.5a.75.75 0 0 1 0-1.5Zm0 5h8.5a.75.75 0 0 1 0 1.5h-8.5a.75.75 0 0 1 0-1.5ZM2 14a1 1 0 1 1 0-2 1 1 0 0 1 0 2Zm1-6a1 1 0 1 1-2 0 1 1 0 0 1 2 0ZM2 4a1 1 0 1 1 0-2 1 1 0 0 1 0 2Z"></path></svg> de menu "Estrutura de Tópicos" no canto superior da página renderizada.

## Links de seção em arquivos markdown e páginas de blob

Você pode criar um link direto para qualquer seção que tenha um título. Para visualizar a âncora gerada automaticamente em um arquivo renderizado, passe o mouse sobre o cabeçalho da seção para expor o ícone <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-link" aria-label="the link" role="img"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg> e clique no ícone para exibir a âncora em seu navegador.

![Captura de tela de um LEIAME de um repositório. À esquerda de um título de seção, um ícone de link é descrito em laranja escuro.](/assets/images/help/repository/readme-links.png)

Para obter informações mais detalhadas sobre links de seção, confira [Links de seção](/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#section-links).

## Links relativos e caminhos de imagem em arquivos markdown

É possível definir links relativos e caminhos de imagens em seus arquivos representados para ajudar os leitores a acessar outros arquivos no repositório.

Um link relativo é um link que é relativo ao arquivo atual. Por exemplo, se você tiver um arquivo LEIAME na raiz do repositório e tiver outro arquivo em *docs/CONTRIBUTING.md*, o link relativo para *CONTRIBUTING.md* no LEIAME poderá ter esta aparência:

```text
[Contribution guidelines for this project](docs/CONTRIBUTING.md)
```

O GitHub transformará automaticamente o link relativo ou o caminho da imagem baseado em qualquer branch em que você estiver no momento para que o link ou o caminho sempre funcione. O caminho do link será relativo ao arquivo atual. Links que começam com `/` serão relativos à raiz do repositório. Você pode usar todos os operandos de link relativos, como `./` e `../`.

O texto do link deve estar em uma única linha. O exemplo abaixo não funcionará.

```markdown
[Contribution
guidelines for this project](docs/CONTRIBUTING.md)
```

Os links relativos são mais fáceis para usuários que clonam o seu repositório. Os links absolutos podem não funcionar em clones do seu repositório - recomendamos usar links relativos para referir-se a outros arquivos no seu repositório.

## Wikis

Um README deve conter apenas as informações necessárias para desenvolvedores começarem a usar e a contribuir com o projeto. A documentação mais longa é mais adequada para wikis. Para saber mais, confira [Sobre wikis](/pt/communities/documenting-your-project-with-wikis/about-wikis).

## Leitura adicional

* [Adicionar um arquivo a um repositório](/pt/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)
* [5 dicas para tornar sua GitHub página de perfil acessível](https://github.blog/2023-10-26-5-tips-for-making-your-github-profile-page-accessible/) no GitHub blog
* [Como facilitar a criação rápida e a retomada de codespaces](/pt/codespaces/setting-up-your-project-for-codespaces/setting-up-your-repository/facilitating-quick-creation-and-resumption-of-codespaces)
