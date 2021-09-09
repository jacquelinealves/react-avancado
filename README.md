# React Avançado

Curso sobre e-commerce real do zero, indo do backend ao frontend.

### O que o NextJS tem/faz?

- Renderização no servidor (Server Side Rendering - SSR)
- Geração de estáticos (Static Site Generation - SSG)
- CSS-in-JS (Styled-jsx, Styled Componentes, Emotion, etc)
- Zero Configuration (rotas, hot reloading, code splitting...)
- Completamente extensível (controle completo do Babel/WebPack, plugins e etc)
- Otimizado para produção

### Tipos de aplicação

- Static Site (SSG)
  HTML/CSS/JS
  Geradores estáticos finais: Gatsby JS, Hero
  _Ps.: O NextJS também permite esta opção_

- Client Side Rendering (SPA) - Create React App

- Server Side Rendering (SSR) - NextJS
  Tem suporte para SSG, SSR e SPA

### GraphQL

Linguagem de consulta de dados
Melhoria da Rest API
Funciona muito bem com React

Vantagens:

- Permite evolução constante
- Rota única
- Entrega apenas dos dados solicitados

### GraphQLClients

Criar camadas de abstração para realizar queries/mutations, sistemas de cache, validações e otimizações.

**Caching Client**
Mais robusto, portanto, é melhor aproveitado em projetos maiores.
Responsável por pegar os dados e colocar nas camadas de cache.
Máquinas de estado (redux de contexto).

Mais conhecidos/utilizados:

1. FetchQL
   Bem leve
   Mais Simples
   API simplificada
   ES2015
   Isomórfico: funciona tanto no Node quanto no Browser

2. GraphQL Request
   Praticamente igual ao FetchQL: simples, leve e isomórfico
   Baseado em Promises (async/await)
   Suporte ao TS

3. uRQL
   Leve e focado em perfomance
   Altamente extensível
   Junto ao Exchanges possui caching
   Suporte offline
   Relativamente novo
   Possui pouca adoção e pouco material online

4. Relay Modern
   Lib bastante consolidade
   Focada em performance
   Pré-compila as queries do GraphQL em build time (evita que o user baixe o parser)
   Sistema de caching/states
   Necessita mais configs no tooling
   Curva de aprendizado maior

5. Apollo Client
   Largamente utilizada no mercado
   Sistema de caching/states
   API simplificada com suporte aos hooks
   Muito material online
   Extremamente grande e com atualizações constantes com Breaking Changes

### Strapi

Headless CMS 100% open-source feito 100% em JS, totalmente customizável (API e painel) e orientado em Agil.

- !! do CMS Tradicional: dados gerenciados por uma API
- Agnóstico de frameworks: funciona em React, Vue, Angular, Rest API ou GraphQL e etc
- Manutenção mais fácil e criação de protótipos mais ágil
- Self Hosted: controle de dados e onde colocá-los

**Features nativas:**

- Suporte a multiplos BD: SQLite, MongoDB, Postgres, MariaDB
- Documentação automática complugin one-click
- Integração com webhooks
- Autenticações e Permissões por padrão
- Integração com diferentes serviços
- Sistema de emails integrado
- Sistema de assets que otimiza imagens e cria em diferentes tamanhos
- Sites estáticos, institucionais, notícias, ecommerce

**3 tipos de estrutura:**

1. Collection Types
   Ex.: usuários, produtos, categorias
2. Single Types
   Ex.: homepage, footer, menu, header
3. Component Types
   Ex.: galerias, hero

### CSS-in-JS

Conjunto de idéias para resolver problemas complexos do CSS.

- Critical CSS automático
- Escopo definido (sem colisão de classes)
- Remoção de CSS não utilizado
- Estilos dinâmicos (props, themes...)
- Manutenção simplificada
- Vendor prefixing automático

**Libs:**

- Styled Components
- Glamor
- Aphrodite
- Emotion
- Styled JSX

### Testes

Funcionam como uma primeira camada de documentação (mas não substitui a mesma)

**Testes unitários**

- Funciona como o dev espera?
- Testes isolados em pequenas unidades de código
- Simula métodos e retornos

**Testes funcionais**

- Funciona como o usuário espera?
- Checa se as unidades funcionam entre si
- Podem conter múltiplas classes, métodos, etc
- Simula ações do usuário
