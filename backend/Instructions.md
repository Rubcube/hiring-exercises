![](../assets/teste-tecnico-backend.png)

## Introdução

Bem-vindo ao nosso teste técnico para a posição de **desenvolvedor back-end**! 

Nosso objetivo é avaliar sua capacidade de resolver problemas, estruturar soluções escaláveis e criar código limpo e bem documentado. 

💡 Aqui estão alguns dos critérios que levamos em consideração ao avaliar sua solução:

- **Testes**: Cobertura de testes unitários e/ou de integração.
- **Deployment**: Facilidade para executar a aplicação localmente ou em ambiente cloud.
- **Documentação**: `README` detalhado explicando a arquitetura e como rodar a aplicação.
  - Inclua detalhes de como utilizar os recursos da API. Por exemplo, disponibilizando as chamadas em `cUrl`.
- **Aderência à stack**: Uso de tecnologias compatíveis com a vaga. Por exemplo, se a vaga é para Node.js com Express, priorizamos essas tecnologias na análise.

---

![](../assets/teste-tecnico-backend-requisitos.png)

### ⏳ Tempo de desenvolvimento
- **Prazo:** 48 horas a partir do recebimento da notificação por e-mail.

### 👾 Tecnologias permitidas
- **Linguagens:** TypeScript, JavaScript, .NET (C#), Ruby e Python.
- **Frameworks:** NestJS, ExpressJS, Fastify, .NET Framework.
- **Banco de dados:** Qualquer banco SQL ou NoSQL é permitido.

---

![](../assets/teste-tecnico-backend-desafio.png)

Você deverá desenvolver uma API que implemente os seguintes recursos:

### 🔗 1. Integração com API Pública
Escolha alguma das APIs públicas para integrar no projeto:
- [OpenWeather](https://openweathermap.org/api) - Previsão do tempo.
- [Metalprice API](https://metalpriceapi.com/documentation#api_convert) - Câmbio de moedas.
- [Rest Countries](https://restcountries.com/) - Dados sobre países.

Sua API deve consumir dados da API pública escolhida e apresentar informações relevantes em um endpoint estruturado.

### 🔐 2. Autenticação
Implemente autenticação utilizando JWT (JSON Web Token). Usuários deverão se registrar e fazer login para acessar determinados recursos protegidos da API.

### 📋 3. Listagem com Filtros
Crie um endpoint para listar dados relevantes da API integrada, permitindo filtros por pelo menos dois critérios diferentes.
* Inclua uma paginação para listar os dados.

### 👥 4. Gerenciamento de Usuários
Implemente endpoints para:
- Criar um usuário.
- Editar um usuário.
- Deletar um usuário.
- Listar um usuário.
- Listar vários usuários (com paginação e filtros)

Os dados podem ser armazenados em banco de dados SQL o NoSQL.

### 📜 5. Consulta de Logs
Registre um histórico de todas as chamadas feitas à API, incluindo informações como usuário, endpoint, data e hora.
* Crie um endpoint para consultar os logs, permitindo filtrar por usuário, data ou endpoint.

---

![](../assets/teste-tecnico-backend-entrega.png)

Para submeter o teste, siga as instruções do repositório: [Instruções de envio](https://github.com/rubcube/hiring-exercises/blob/master/README.md).

O que esperamos na entrega:
- Código hospedado em um repositório público do `GitHub` ou `GitLab`.
- Um `README.md` bem documentado com:
  - Instruções de instalação e execução.
  - Explicação sobre as decisões técnicas tomadas.
  - Exemplo de chamadas para os endpoints.
- *Opcional*: Deploy da API em um serviço cloud (Heroku, Vercel, Render, AWS, etc.).

---

![](../assets/teste-tecnico-backend-consideracoes.png)

Buscamos um código bem estruturado, testável e bem documentado. Lembre-se de que simples é melhor do que complexo e de que clareza é essencial. 

Boa sorte! 🚀