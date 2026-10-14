# AthletaNexus — Front-end responsivo

Projeto feito com HTML, CSS e JavaScript puro, sem frameworks ou instalação de dependências.

## Como executar
1. Extraia `AthletaNexus-front-end.zip`.
2. Abra a pasta `athletanexus-web` no Visual Studio Code.
3. Abra `index.html` no navegador. Para uma experiência mais previsível durante o desenvolvimento, use a extensão Live Server.

## Fluxo de conta implementado
- O site inicia na tela de login, sem usuário ou conta previamente cadastrada.
- É possível alternar entre login e criação de conta.
- O cadastro solicita nome, tipo de perfil, e-mail, senha, confirmação de senha e aceite dos termos.
- O sistema valida e-mail duplicado, senha mínima de 8 caracteres e confirmação da senha.
- O login confere o e-mail e a senha cadastrados; credenciais incorretas mostram uma mensagem de erro.
- A sessão fica ativa durante a navegação e recarregamentos da mesma aba; sair encerra a sessão.
- O perfil editado é guardado localmente e carregado ao entrar novamente.
- As contas são armazenadas no `localStorage` deste navegador, e a senha é guardada como hash no protótipo.

## Telas incluídas
- Login e cadastro sem conta pré-criada
- Visão geral / dashboard
- Descoberta de atletas com pesquisa e filtros
- Perfis de atletas em modal
- Matches e interesses
- Oportunidades com filtros e registro local de interesse
- Mensagens demonstrativas
- Perfil editável
- Configurações e saída da conta
- Layout responsivo para computador, tablet e celular

## Limitações importantes
Esta é uma demonstração front-end. O cadastro não cria uma conta em servidor e os dados ficam somente no navegador em que foram cadastrados. A função de hash no navegador não substitui autenticação segura de produção; a versão pública deve usar API, banco de dados, hash de senha no servidor (por exemplo Argon2id ou bcrypt), recuperação de senha, validação, controle de sessão e autorização. As mensagens, métricas, perfis de terceiros e oportunidades são dados fictícios de demonstração e não representam usuários ou eventos reais.

Para limpar as contas de teste, abra as ferramentas de desenvolvedor do navegador e apague a chave `athletanexus_accounts_v1` do armazenamento local do site.

## Arquivos
- `index.html`: estrutura da aplicação
- `style.css`: visual, layout e responsividade
- `app.js`: navegação, validações, cadastro, login e interações
- `README.md`: instruções e limitações
