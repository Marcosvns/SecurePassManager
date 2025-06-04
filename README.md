# 🔐 **SecurePassManager**

> Um gerenciador de senhas moderno e seguro feito em **Java**, com **criptografia avançada**, **2FA** e suporte a múltiplos usuários.

<p align="center">
  <img src="https://img.shields.io/badge/Java-17-orange.svg" alt="Java">
  <img src="https://img.shields.io/badge/Maven-3.6+-blue.svg" alt="Maven">
  <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License">
  <img src="https://img.shields.io/badge/Security-AES%2Fbcrypt-yellow.svg" alt="Security">
  <img src="https://img.shields.io/badge/2FA-TOTP%20%7C%20QR%20Code-blueviolet.svg" alt="2FA">
</p>

---

## ✨ **Destaques do Projeto**

### 🔒 Armazenamento Seguro
- Criptografia **AES-256-GCM**
- Hashing com **bcrypt** para senhas mestras
- Proteção contra **força bruta**
- Gerenciamento de **chaves criptográficas**

### 🔐 Autenticação Avançada
- **2FA** com TOTP + QR Code
- Códigos de **backup** para recuperação
- Detecção de login malicioso

### 🛡️ Segurança Proativa
- Verificação de vazamentos com **HaveIBeenPwned**
- Gerador de **senhas fortes**
- Validação da força da senha
- Proteção contra **SQL Injection**

### 👥 Multiusuário
- Isolamento completo entre contas
- Gerenciamento de permissões por usuário

---

## 🚀 **Como Começar**

### ✅ Pré-requisitos
- Java 17+
- Maven 3.6+
- MongoDB 4.4+ rodando localmente (`localhost:27017`)

## 🛠️ Instalação


### -Clone o projeto
   ```bash
   git clone https://github.com/Marcosvns/SecurePassManager
   cd SecurePassManager
   ```

### -Compile o projeto
   ```bash
   mvn clean install
   ```

### -Execute o app
   ```bash
   mvn exec:java -Dexec.mainClass="com.securepassmanager.Main"
   ```

## 📁 Estrutura do Projeto

```
src/
├── main/
│   └── java/com/securepassmanager/
│       ├── model/        # Entidades e DTOs
│       ├── service/      # Regras de negócio
│       ├── security/     # Módulos de segurança
│       ├── util/         # Utilitários gerais
│       └── api/          # Integrações externas
└── test/
    └── java/com/securepassmanager/
        └── ...           # Testes unitários e integração

```
## ⚙️ Configuração

O sistema utiliza as seguintes configurações padrão:

- MongoDB: `mongodb://localhost:27017`
- Coleções: `users`, `passwords`, `master_password`
- Banco: `SecurePassManager`

Para customizações, crie um `application.properties` na raiz do projeto.

## 🔐 Detalhes de Segurança

🔑 Criptografia

- AES-256-GCM + geração segura de chaves
- bcrypt para hashing de senhas mestras

🧾 Autenticação

- 2FA com TOTP + QR Code
- Tentativas limitadas e bloqueio automático
- Códigos de backup para recuperação

## 🤝 Contribua com o Projeto

- Faça um fork
- Crie uma branch: git checkout -b feature/NovaFuncionalidade
- Commit suas alterações: git commit -m 'feat: adiciona nova funcionalidade'
- Push: git push origin feature/NovaFuncionalidade
- Abra um Pull Request 🚀


## 📝 Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para detalhes.

## 📧 Contato

Marcos Vinícius marcosvn0803@gmail.com

