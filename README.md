# 🐳 Ambiente Docker Local para Aplicações PHP + NGINX + MySQL

Este ambiente foi criado para facilitar o desenvolvimento local de aplicações PHP utilizando NGINX, PHP-FPM 8.1, MySQL 8 e PHPMyAdmin.

---

## ⚙️ Tecnologias Utilizadas

- **NGINX (alpine)** — Servidor web 
- **PHP-FPM 8.1** — Interpretador PHP
- **MySQL 8.0** — Banco de dados relacional
- **PHPMyAdmin** — Interface web para administração do MySQL
- **Docker Compose 3.8** — Orquestração

---


---

## 🆕 Novas Funcionalidades

✅ **Atualização para PHP 8.1**  
✅ **Uso de `fastcgi.conf` + `fastcgi_split_path_info`** para melhor compatibilidade com frameworks modernos  
✅ **Volumes nomeados (`app`, `mysql_data`)** para maior segurança e performance  
✅ **Healthchecks** para garantir que os serviços estejam funcionando corretamente  
✅ **`client_max_body_size`** configurado para uploads maiores  
✅ **Bloqueio de execução de arquivos PHP em diretórios públicos**  
✅ **Redes isoladas (`webnet`)** entre os containers  

---

## 📦 Como Utilizar

### 1. Configure o arquivo `.env`

Crie um arquivo `.env` na raiz com:

```env
PASSWORD_ROOT=suasenhasegura
DATABASE=meubanco
DBUSER=usuario
DBPASSWORD=senhadousuario
```

### 2. Suba o ambiente


```env
docker compose up -d 
```