# ⚽ LaPelota - Gestão de Peladas

Sistema completo para gerenciar peladas de futebol, com controle de jogadores, times, filas de espera e placar em tempo real.

![Vue 3](https://img.shields.io/badge/Vue.js-3.x-4FC08D?logo=vue.js)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS-38B2AC?logo=tailwind-css)
![Supabase](https://img.shields.io/badge/Supabase-Database-3ECF8E?logo=supabase)

## ✨ Funcionalidades

- 🔐 **Autenticação** - Login e cadastro de usuários via Supabase Auth
- 👥 **Grupos** - Crie e gerencie grupos de pelada
- 📧 **Convites** - Convide jogadores por e-mail para participar dos grupos
- ⚽ **Gestão de Pelada** - Controle completo de partidas:
  - Cadastro de jogadores e goleiros
  - Controle de pagamento e presença
  - Fila de espera inteligente
  - Sorteio automático de times
  - Placar e cronômetro em tempo real
  - Rotação automática de jogadores
- 💾 **Persistência** - Dados salvos localmente por grupo/usuário

## 🚀 Como Rodar Localmente

### Pré-requisitos

1. Uma conta no [Supabase](https://supabase.com) (gratuito)
2. Um navegador moderno (Chrome, Firefox, Edge, etc.)

### Passo a Passo

1. **Clone o repositório**

```bash
git clone https://github.com/seu-usuario/lapelota.git
cd lapelota
```

2. **Configure o Supabase**

   - Acesse [supabase.com](https://supabase.com) e crie um novo projeto
   - Vá em **Project Settings** > **API**
   - Copie a `URL` e a `anon public` key

3. **Configure as credenciais**

   - Copie o arquivo de exemplo:

```bash
cp config.example.js config.js
```

   - Edite o arquivo `config.js` e preencha com suas credenciais:

```javascript
const CONFIG = {
    SUPABASE_URL: 'https://seu-projeto.supabase.co',
    SUPABASE_ANON_KEY: 'sua-anon-key-aqui'
};
```

5. **Abra o projeto**

   Simplesmente abra o arquivo `index.html` no seu navegador!

   > 💡 **Dica**: Você pode usar a extensão "Live Server" do VS Code para uma melhor experiência de desenvolvimento.

## 📁 Estrutura do Projeto

```
lapelota/
├── index.html          # Aplicação principal (Vue 3 + Tailwind)
├── config.js           # Credenciais do Supabase (não versionado)
├── config.example.js   # Template de configuração
├── .gitignore          # Arquivos ignorados pelo Git
└── README.md           # Este arquivo
```

## 🛠️ Tecnologias

- **Vue 3** - Framework JavaScript (via CDN)
- **Tailwind CSS** - Framework CSS utilitário (via CDN)
- **Supabase** - Backend as a Service (Auth + Database)
- **Phosphor Icons** - Biblioteca de ícones