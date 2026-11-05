# João Adolfo

Estudante de Engenharia de Software na UVA e fundador da [Valtrea](https://www.valtrea.com.br), no Rio de Janeiro.
Desenvolvo produtos completos (API, site e app Android), do banco de dados ao deploy, com segurança, LGPD e testes
automatizados. Hoje mantenho quatro produtos próprios no ar.

[![Site](https://img.shields.io/badge/valtrea.com.br-55B02E?style=flat-square&logo=googlechrome&logoColor=white)](https://www.valtrea.com.br)
[![E-mail](https://img.shields.io/badge/contato@valtrea.com.br-1C2026?style=flat-square&logo=gmail&logoColor=white)](mailto:contato@valtrea.com.br)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jo%C3%A3o-adolfo/)

## Em destaque: Valtrea Finance

App de finanças pessoais em produção em **[finance.valtrea.com.br](https://finance.valtrea.com.br)**.
Construído do zero por mim: front-end, API, banco de dados, infraestrutura e segurança.

- Saldo por período, gastos por categoria, evolução mês a mês e orçamento mensal
- Contas fixas lançadas automaticamente, sem duplicidade
- Login com JWT e renovação de sessão, confirmação de e-mail, recuperação de senha e bloqueio contra força bruta
- API REST documentada com Swagger e testada de ponta a ponta a cada push
- Deploy contínuo, monitoramento de erros, backup diário criptografado e app instalável (PWA)

**[Ver detalhes do projeto →](https://github.com/adolfo-araujo/valtrea-finance)**

## Outros produtos da Valtrea

Abertos para testes, cada um com API em Java e Spring Boot, site em React e app Android em Kotlin.

### [Valtrea Volta](https://volta.valtrea.com.br): se perdeu, pode voltar

Etiquetas com QR Code para mochilas, chaves, carteiras e outros objetos. Quem encontra lê o código com a câmera do
celular e avisa o dono pela página da etiqueta, sem ver o nome, o telefone ou o endereço dele.

- Cadastro de objetos e etiquetas com código aleatório de 256 bits, guardado só como hash e cifrado (AES-256-GCM)
- Modo "perdi este objeto", que mostra um destaque para quem ler o QR Code
- Avisos de quem encontrou com aceite, proteção contra robôs e limite por pessoa e por objeto
- QR Code para imprimir no site e para salvar como imagem no app

**[Ver o código →](https://github.com/adolfo-araujo/valtrea-volta)**

### [Valtrea Pulso](https://pulso.valtrea.com.br): a voz organizada do seu bairro

Moradores registram o que o bairro precisa (iluminação, limpeza, trânsito, praças), reúnem o apoio dos vizinhos e
acompanham o que acontece com cada iniciativa até ser resolvida.

- Bairros criados pelos próprios moradores, sem duplicados (nomes iguais com ou sem acento viram o mesmo bairro)
- Um apoio por pessoa e lista ordenada pelas iniciativas mais apoiadas
- Linha do tempo com as novidades e as fases: aberta, em andamento, resolvida
- Moderação: com três denúncias a iniciativa some até a revisão no painel; em público aparece só o primeiro nome

**[Ver o código →](https://github.com/adolfo-araujo/valtrea-pulso)**

### [Valtrea Agora](https://agora.valtrea.com.br): oportunidades que acontecem perto de você

Horários vagos de salões, barbearias e outros serviços da região, para reservar no mesmo dia. O estabelecimento
publica os horários que ficaram livres e o cliente reserva com um toque, sem pagar nada pelo app.

- Todo estabelecimento passa por análise antes de aparecer, e denúncias o levam de volta para a fila
- Reserva segura mesmo com cliques ao mesmo tempo: trava da linha no banco e índice único (testado com concorrência)
- Agenda do estabelecimento com cancelamento pelos dois lados, avisos por e-mail e controle de presença
- O estabelecimento vê só o primeiro nome do cliente e o telefone, se ele quiser informar

**[Ver o código →](https://github.com/adolfo-araujo/valtrea-agora)**

Em desenvolvimento: **Valtrea Pay**, pagamentos integrados ao Finance.

O que esses projetos têm em comum:

- Testes de integração com PostgreSQL real, testes de tela no Android e testes no navegador (computador e celular) com verificação de acessibilidade, a cada push
- Testes de carga, varredura de dependências vulneráveis e de segredos no código no CI
- LGPD na prática: exportação dos dados, exclusão da conta na hora, retenção automática e registro das operações
- Proteção contra abuso: limites por IP, bloqueio de login, confirmação de e-mail e controle de acesso por recurso

## Tecnologias

**Front-end**
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-0F172A?style=flat-square&logo=tailwindcss&logoColor=38BDF8)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

**Back-end e dados**
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

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
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=black)
![Sentry](https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white)
![Neon](https://img.shields.io/badge/Neon-00E599?style=flat-square&logo=neon&logoColor=black)

## O que estou fazendo agora

- Validando o Finance, o Volta, o Pulso e o Agora com os primeiros usuários
- Preparando os apps Android para a Play Store e terminando o Valtrea Pay
- Atendendo empresas com sites e sistemas sob medida pela Valtrea

## Contato

Aberto a conversas sobre projetos e parcerias: **contato@valtrea.com.br**
