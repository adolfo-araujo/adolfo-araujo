# João Adolfo

**Desenvolvedor full stack · Estudante de Engenharia de Software (UVA) · Fundador da [Valtrea](https://www.valtrea.com.br)**

Rio de Janeiro, Brasil. Desenvolvo produtos completos (API, site e app Android), do banco de dados ao deploy, com
segurança, LGPD e testes automatizados. Hoje mantenho quatro produtos próprios e o site da Valtrea no ar, e na
graduação construo projetos em Java, Python, C e PHP.

[![Site](https://img.shields.io/badge/valtrea.com.br-55B02E?style=flat-square&logo=googlechrome&logoColor=white)](https://www.valtrea.com.br)
[![E-mail](https://img.shields.io/badge/contato@valtrea.com.br-1C2026?style=flat-square&logo=gmail&logoColor=white)](mailto:contato@valtrea.com.br)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jo%C3%A3o-adolfo/)

## Em destaque: Valtrea Finance

App de finanças pessoais em produção em **[finance.valtrea.com.br](https://finance.valtrea.com.br)**.
Construído do zero por mim: front-end, API, banco de dados, infraestrutura e segurança.

- Saldo por período, gastos por categoria, evolução mês a mês e orçamento mensal
- Contas fixas lançadas automaticamente, sem duplicidade
- Valtrea Assistente: chat que lança gastos escritos em linguagem natural, entende o contexto da conversa e aprende com o usuário, sem IA externa (regras, pontuação de confiança e base de conhecimento próprias)
- Login com JWT e renovação de sessão, confirmação de e-mail, recuperação de senha e bloqueio contra força bruta
- API REST documentada com Swagger e testada de ponta a ponta a cada push
- Deploy contínuo, monitoramento de erros, backup diário criptografado e app instalável (PWA)

**[Acessar o Valtrea Finance →](https://finance.valtrea.com.br)**

## Site da Valtrea

Site institucional em **[valtrea.com.br](https://www.valtrea.com.br)**, em português e inglês, rodando na borda da
Cloudflare. Monorepo TypeScript com site em Astro e API e coleta de dados em Cloudflare Workers com Hono, adaptado
a partir da estrutura do projeto open source [Devlytics](https://github.com/gabrueldev/devlytics) (licença MIT).
Código em **[adolfo-araujo/valtrea-site](https://github.com/adolfo-araujo/valtrea-site)**.

- Estatísticas próprias sem cookies: a visita é contada com um código diário descartável e o IP não é gravado
- Painel com login pelo GitHub, visitas por dia, atenção por seção e links rastreados com aviso por e-mail
- Apoio com café por Pix ou cartão via Cakto: o cartão é protegido no navegador e o pagamento é confirmado por webhook
- Cinco lojas de demonstração (pousada, achadinhos, corrida, pet shop e cardápio digital) com carrinho e pedido
- Política de privacidade, termos e declaração de acessibilidade escritos a partir do que o código realmente faz

## Outros produtos da Valtrea

Abertos para testes, cada um com API em Java e Spring Boot, site em React e app Android em Kotlin. O código é privado; os sites estão no ar para usar.

### [Valtrea Volta](https://volta.valtrea.com.br): se perdeu, pode voltar

Etiquetas com QR Code para mochilas, chaves, carteiras e outros objetos. Quem encontra lê o código com a câmera do
celular e avisa o dono pela página da etiqueta, sem ver o nome, o telefone ou o endereço dele.

- Cadastro de objetos e etiquetas com código aleatório de 256 bits, guardado só como hash e cifrado (AES-256-GCM)
- Modo "perdi este objeto", que mostra um destaque para quem ler o QR Code
- Avisos de quem encontrou com aceite, proteção contra robôs e limite por pessoa e por objeto
- QR Code para imprimir no site e para salvar como imagem no app

### [Valtrea Pulso](https://pulso.valtrea.com.br): a voz organizada do seu bairro

Moradores registram o que o bairro precisa (iluminação, limpeza, trânsito, praças), reúnem o apoio dos vizinhos e
acompanham o que acontece com cada iniciativa até ser resolvida.

- Bairros criados pelos próprios moradores, sem duplicados (nomes iguais com ou sem acento viram o mesmo bairro)
- Um apoio por pessoa e lista ordenada pelas iniciativas mais apoiadas
- Linha do tempo com as novidades e as fases: aberta, em andamento, resolvida
- Moderação: com três denúncias a iniciativa some até a revisão no painel; em público aparece só o primeiro nome

### [Valtrea Agora](https://agora.valtrea.com.br): oportunidades que acontecem perto de você

Horários vagos de salões, barbearias e outros serviços da região, para reservar no mesmo dia. O estabelecimento
publica os horários que ficaram livres e o cliente reserva com um toque, sem pagar nada pelo app.

- Todo estabelecimento passa por análise antes de aparecer, e denúncias o levam de volta para a fila
- Reserva segura mesmo com cliques ao mesmo tempo: trava da linha no banco e índice único (testado com concorrência)
- Agenda do estabelecimento com cancelamento pelos dois lados, avisos por e-mail e controle de presença
- O estabelecimento vê só o primeiro nome do cliente e o telefone, se ele quiser informar

Em desenvolvimento: **Valtrea Pay**, pagamentos integrados ao Finance.

O que esses projetos têm em comum:

- Testes de integração com PostgreSQL real, testes de tela no Android e testes no navegador (computador e celular) com verificação de acessibilidade, a cada push
- Testes de carga, varredura de dependências vulneráveis e de segredos no código no CI
- LGPD na prática: exportação dos dados, exclusão da conta na hora, retenção automática e registro das operações
- Proteção contra abuso: limites por IP, bloqueio de login, confirmação de e-mail e controle de acesso por recurso

## Projetos acadêmicos

Desenvolvidos no curso de Engenharia de Software da Universidade Veiga de Almeida (UVA). Todos têm README com
instruções de execução, telas e decisões técnicas.

| Projeto | Descrição | Tecnologias |
|---|---|---|
| [**Conexão Edu**](https://github.com/adolfo-araujo/conexao-edu-backend) | Plataforma educacional com API REST, autenticação JWT e eventos assíncronos a cada cadastro ou alteração, com painel de monitoramento. *Desenvolvimento Backend, 2026, em equipe.* | Java 17, Spring Boot 3, Spring Security, RabbitMQ, Docker |
| [**Autenticação LDAP com Docker**](https://github.com/adolfo-araujo/ldap-auth-docker) | API que autentica usuários num diretório OpenLDAP, emite JWT e libera rotas por grupo. Quatro serviços em Docker Compose com redes separadas e healthcheck. *Desenvolvimento Backend, 2026, individual.* | Python, Flask, OpenLDAP, JWT, Nginx, Docker |
| [**Leiturinha**](https://github.com/adolfo-araujo/Site-Leiturinha) | Sistema web de catálogo de livros com busca, favoritos, formulário de contato e CRUD completo. *Desenvolvimento Web, em equipe.* | PHP (PDO), MySQL, HTML, CSS, JavaScript |
| [**Paradigmas de Programação**](https://github.com/adolfo-araujo/paradigmas-programacao) | Os mesmos problemas resolvidos em C, Python e Java para comparar os paradigmas estruturado e orientado a objetos, com validação automática no GitHub Actions. | C, Python, Java |
| [**Loja de Calçados**](https://github.com/adolfo-araujo/loja-de-calcados-c) | Calculadora de compras em linha de comando: catálogo, frete por região e peso, resumo do pedido e previsão de entrega, com testes automatizados. *Bases de Programação, 2025.* | C, Python (testes) |

**Primeiros estudos (2025):** gerador de senhas em três versões, [Python estruturado](https://github.com/adolfo-araujo/Gerador-de-Senha-Paradigma-estruturado-),
[Python orientado a objetos](https://github.com/adolfo-araujo/Python-Orientado-ao-Objeto) e [Java](https://github.com/adolfo-araujo/Java-),
e uma [calculadora com interface gráfica](https://github.com/adolfo-araujo/Calculado-Simples) em Python com Tkinter.

## Tecnologias

**Front-end**
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-0F172A?style=flat-square&logo=tailwindcss&logoColor=38BDF8)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Astro](https://img.shields.io/badge/Astro-BC52EE?style=flat-square&logo=astro&logoColor=white)

**Back-end e dados**
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Hono](https://img.shields.io/badge/Hono-E36002?style=flat-square&logo=hono&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=black)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)

**Mobile**
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack_Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white)
![Android](https://img.shields.io/badge/Android-34A853?style=flat-square&logo=android&logoColor=white)

**Testes e qualidade**
![JUnit](https://img.shields.io/badge/JUnit-25A162?style=flat-square&logo=junit5&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![k6](https://img.shields.io/badge/k6-7D64FF?style=flat-square&logo=k6&logoColor=white)

**Infraestrutura**
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare_Workers-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=black)
![Sentry](https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white)
![Neon](https://img.shields.io/badge/Neon-00E599?style=flat-square&logo=neon&logoColor=black)

## O que estou fazendo agora

- Validando o Finance, o Volta, o Pulso e o Agora com os primeiros usuários
- Preparando os apps Android para a Play Store e terminando o Valtrea Pay
- Atendendo empresas com sites e sistemas sob medida pela Valtrea
- Evoluindo o painel de estatísticas do site para outros sites usarem

## Formação

**Engenharia de Software** · Universidade Veiga de Almeida (UVA), Rio de Janeiro · em andamento, desde 2025

## Contato

Aberto a conversas sobre projetos e parcerias: **contato@valtrea.com.br**
