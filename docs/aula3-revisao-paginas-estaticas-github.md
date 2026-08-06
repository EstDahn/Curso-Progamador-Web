# Aula 3: Revisão - Páginas Estáticas no GitHub (GitHub Pages)

## O que são Páginas Estáticas?
Uma página estática é um site entregue ao navegador do usuário exatamente da mesma forma como está armazenado no servidor. Ela não possui processamento de back-end (como PHP, Python, Java ou Node.js) operando no servidor para gerar o conteúdo no momento do acesso, tampouco utiliza banco de dados. O conteúdo é construído utilizando apenas tecnologias executadas no lado do cliente (no navegador):
- HTML (estrutura da página)
- CSS (estilo e formatação visual)
- JavaScript (interatividade e comportamento)

## O que é o GitHub Pages?
O GitHub Pages é um serviço de hospedagem de sites estáticos oferecido de forma nativa e gratuita pelo GitHub. Ele permite que você publique um site na internet diretamente de um repositório da sua conta. É uma ferramenta amplamente utilizada para hospedar documentações de projetos, currículos, portfólios, blogs pessoais ou apresentações de análises e tutoriais.

Existem dois tipos principais de sites no GitHub Pages:
1. **Sites de usuário ou organização:** O repositório deve ser obrigatoriamente nomeado no formato `seunomedeusuario.github.io`. Este será o seu site principal.
2. **Sites de projeto:** O site fica vinculado a um repositório de um projeto específico existente e é publicado em um subdiretório, seguindo o padrão `seunomedeusuario.github.io/nome-do-projeto`.

## Passo a Passo para Criar uma Página Estática no GitHub

### Passo 1: Criar o Repositório
1. Acesse sua conta no GitHub.
2. Clique no botão "New" (Novo) para criar um novo repositório.
3. Nomeie o repositório. Para criar seu site de usuário principal, o nome deve ser exatamente `seunomedeusuario.github.io`.
4. Mantenha o repositório como "Public" (Público), pois repositórios privados exigem uma assinatura paga do GitHub para utilizar o recurso do GitHub Pages.
5. Clique em "Create repository" (Criar repositório).

### Passo 2: Adicionar os Arquivos do Site
Você pode enviar arquivos já prontos do seu computador local ou criá-los diretamente na interface web do GitHub.
1. Crie um arquivo com o nome exato de `index.html`. Este arquivo será reconhecido automaticamente como a página inicial (home) do seu site.
2. Escreva a estrutura básica do seu documento HTML dentro deste arquivo.
3. Você pode adicionar outros arquivos e pastas conforme a necessidade do projeto, como uma pasta para imagens, um arquivo `style.css` para a formatação e arquivos `.js` para scripts.
4. Faça o commit (salvamento) dessas alterações na sua branch principal.

### Passo 3: Ativar o GitHub Pages (Para sites de projeto)
Se você estiver criando uma página para um projeto específico (e não o repositório principal `.github.io`, cujo deploy é automático na maioria das vezes):
1. Acesse a aba "Settings" (Configurações) do seu repositório.
2. No menu lateral esquerdo, clique na opção "Pages".
3. Na seção "Build and deployment" (Construção e implantação), selecione a fonte (Source) como "Deploy from a branch".
4. Selecione a branch de onde o site será lido (geralmente `main` ou `master`) e a pasta raiz (`/root`).
5. Clique em "Save" (Salvar).
6. O GitHub fará o processo de build do site e, em seguida, exibirá um link na parte superior da página indicando o endereço onde seu site está publicado. Pode levar alguns minutos para a página ficar totalmente acessível na primeira vez.

## Vantagens de usar o GitHub Pages
- **Custo zero:** A hospedagem é gratuita, o que é ideal para estudantes, desenvolvedores independentes e pequenos projetos.
- **Controle de Versão nativo:** Todo o histórico de alterações do site fica registrado no sistema Git. Se uma atualização quebrar o site, é muito fácil reverter para a versão anterior.
- **Integração direta:** Não é necessário configurar servidores FTP, painéis de controle de hospedagem (como cPanel) ou lidar com infraestrutura. Tudo é feito via comandos Git ou pela própria interface do GitHub.
- **Domínios personalizados:** Apesar de oferecer um endereço gratuito (`.github.io`), é possível configurar um domínio próprio (como `www.meusite.com.br`) apontando para as configurações de DNS do seu GitHub Pages.

## Conclusão
Hospedar páginas estáticas no GitHub é uma das formas mais práticas, eficientes e seguras de colocar projetos web no ar. O domínio dessa ferramenta é uma habilidade fundamental para desenvolvedores, profissionais da área de tecnologia e estudantes que precisam apresentar projetos, compartilhar códigos e documentações em uma infraestrutura confiável.
