# Task List (Laravel 10)

Aplicação CRUD simples construída com Laravel 10 para gerenciar tarefas. Este repositório foi usado em um contexto de aprendizagem e demonstra funcionalidades básicas do framework com Tailwind CSS e Alpine.js.

---

## 🛠️ Tecnologias Utilizadas

- **PHP 8.x**
- **Laravel 10** (MVC framework)
- **Tailwind CSS** para estilização utilitária
- **Alpine.js** para interatividade leve (fechar mensagens flash)
- **SQLite/MySQL** (configurável em `.env`) para banco de dados
- **Composer** para gerenciamento de dependências
- **Vite** como build tool para assets
- **PHPUnit** para testes unitários/funcionais

---

## 🚀 Como rodar o projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/GabrielZanini04/task-list.git
   cd task-list
   ```
2. Instale as dependências PHP e JavaScript:
   ```bash
   composer install
   npm install
   ```
3. Configure o ambiente:
   - Copie `.env.example` para `.env`.
   - Ajuste as credenciais do banco (`DB_CONNECTION`, `DB_HOST`, etc.).
   - Gere a chave do aplicativo:
     ```bash
     php artisan key:generate
     ```
4. Execute migrações e seeders (se houver):
   ```bash
   php artisan migrate
   php artisan db:seed
   ```
5. Compile assets (modo desenvolvimento):
   ```bash
   npm run dev
   ```
6. Inicie o servidor de desenvolvimento:
   ```bash
   php artisan serve
   ```
7. Acesse `http://localhost:8000` no navegador.

> Se estiver usando Docker ou Laragon, ajuste os comandos conforme necessário.

---

## 📁 Estrutura do Projeto

- `app/` – lógica de aplicação (Models, Controllers, Requests)
- `resources/views/` – views Blade para interface
- `routes/web.php` – rotas principais
- `database/migrations/` – definições de tabelas
- `tests/` – casos de teste de exemplo

---

## 💡 Técnicas e Padrões Demonstrados

- Uso de controllers e requests para validação.
- Templates Blade com slots e componentes simples.
- Exibição de mensagens flash com Alpine.js para interação e Tailwind para estilos.
- Organização de CSS utilitário via `@apply` em estilos internos.
- Uso de factories para geração de dados de teste.
- Convenções RESTful para rotas de CRUD.
- Testes básicos com PHPUnit para garantir comportamento.

---

## 📦 Dependências Principais

```json
// exemplo retirado de composer.json
"require": {
    "php": "^8.1.0",
    "fideloper/proxy": "^4.4",
    "fruitcake/laravel-cors": "^2.0",
    "laravel/framework": "^10.0",
    "laravel/sanctum": "^3.2",
    "laravel/tinker": "^2.8"
},

"devDependencies": {
    "laravel/pint": "^1.0",
    "phpunit/phpunit": "^10.0"
}
```


---

## ✔️ Contribuições

Este é um projeto de aprendizado. Sinta-se livre para abrir issues ou pull requests com melhorias, correções ou novas funcionalidades.

---

## 📄 Licença

Sem licença específica. Utilize conforme desejar.
