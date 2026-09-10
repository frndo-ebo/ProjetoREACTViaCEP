# 🗺️ ViaCEP Finder - Fullstack Hub

> Uma aplicação fullstack completa e otimizada que consome a API do ViaCEP. O backend atua como um proxy seguro e inteligente, tratando os dados e aplicando cache, enquanto o frontend entrega uma interface fluida, responsiva e com excelente experiência de usuário (UX).

---

## 🚀 Funcionalidades Coração do Projeto

- **Busca Instantânea:** Digite o CEP e os dados de endereço aparecem num piscar de olhos.
- **Tratamento de Erros:** Identifica CEPs inexistentes ou formatos inválidos antes mesmo de quebrar a aplicação.
- **Backend Seguro:** Chamadas externas centralizadas no servidor, protegendo as regras de negócio.
- **Auto-preenchimento:** Interface inteligente que limpa ou preenche campos dinamicamente.

---

## 🛠️ Arquitetura e Tecnologias

O projeto foi dividido em duas partes fundamentais para manter o código limpo, modular e escalável:

### 💻 Frontend
- **React.js** (com Vite para um ecossistema ultra rápido)
- **CSS Modules** para uma estilização moderna e limpa

### ⚙️ Backend
- **Node.js** com **Express** como servidor base
- **Cors** liberado para comunicação segura com o front
- Integração direta com a API pública do [ViaCEP](https://viacep.com.br)

---

## 📦 Como Rodar a Aplicação na Sua Máquina

### Pre-requisitos
Antes de começar, você precisa ter instalado em sua máquina o [Node.js](https://nodejs.org) e um gerenciador de pacotes (npm ou yarn).

### 1. Clonando o Repositório
```bash
git clone https://github.com
cd seu-repositorio-viacep
```

### 2. Configurando o Backend ⚙️
```bash
# Navegue até a pasta do servidor
cd backend

# Instale as dependências
npm install

# Inicie o servidor de desenvolvimento
npm run dev
# O servidor backend iniciará por padrão na porta http://localhost:3001 (ou na porta configurada)
```

### 3. Configurando o Frontend 💻
```bash
# Abra uma nova aba no seu terminal e navegue até a pasta do cliente
cd frontend

# Instale as dependências
npm install

# Inicie a aplicação React
npm run dev
# O Vite abrirá a aplicação em uma porta local, geralmente http://localhost:5173
```

---

## 🗺️ Estrutura de Pastas do Projeto

```text
seu-repositorio-viacep/
├── backend/
│   ├── src/
│   │   ├── controllers/   # Regras de negócio e chamadas ao ViaCEP
│   │   └── server.js      # Inicialização do Express
│   └── package.json
│
└── frontend/
    ├── src/
    │   ├── components/    # Componentes reutilizáveis (Card, Form, etc.)
    │   ├── App.jsx        # Componente principal
    │   └── main.jsx       # Ponto de entrada do React
    └── package.json
```

---

## 🔗 Endpoints do Backend

Caso queira testar as rotas do backend isoladamente usando ferramentas como Postman ou Insomnia:

| Método | Endpoint | Descrição | Exemplo de Retorno |
| :--- | :--- | :--- | :--- |
| `GET` | `/api/cep/:cep` | Busca o endereço correspondente ao CEP informado | `{ "logradouro": "Praça da Sé", ... }` |

---

## 🤝 Como Contribuir

Fique à vontade para deixar o projeto ainda mais completo!
1. Faça um **Fork** do projeto.
2. Crie uma nova Feature Branch (`git checkout -b feature/MinhaFeature`).
3. Faça o **Commit** de suas alterações (`git commit -m 'Adicionando uma feature incrível'`).
4. Envie para o repositório original (`git push origin feature/MinhaFeature`).
5. Abra um **Pull Request**.

---


<p align="center">
  Desenvolvido com 💜 por <a href="https://github.com">Fernando</a>
</p>
