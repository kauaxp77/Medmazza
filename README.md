<h1 align="center">
  MedMazza - Agendamento Médico
</h1>

<p align="center">
  <strong>Plataforma robusta para gestão e agendamento de consultas médicas online.</strong>
</p>

## 💻 Sobre o Projeto

O **MedMazza** é um sistema para estruturar e digitalizar a organização de consultas em consultórios médicos ou clínicas. A plataforma suporta três níveis distintos de usuários: **Administradores**, **Médicos** e **Pacientes**. O projeto foi concebido para simplificar a jornada de marcação e também fornecer um poderoso dashboard analítico com as rotinas da clínica.

Este projeto é um excelente demonstrativo da minha proficiência do back-end utilizando PHP e dos conceitos avançados de frameworks MVC modernos.

## 🚀 Tecnologias Utilizadas

O backend e front-end foram construídos visando a estabilidade e segurança.

- **PHP 7 / 8** com framework **Laravel 6.x**
- **MySQL** como banco de dados principal
- Arquitetura **MVC** (Model-View-Controller)
- **Eloquent ORM** para manipulação intuitiva e segura do banco 
- Migrations e Seeders
- Front-end robusto, com estilizações em CSS, HTML5 e interações.

## 📊 Regras de Negócio e Funcionalidades

O sistema tem diversas interações entre papéis:

1. **Paciente**:
   - Cria sua conta, faz login e visualiza um painel próprio (Dashboard).
   - Pode navegar pela lista de médicos disponíveis.
   - Solicita agendamentos e recebe o status das marcações efetuadas ou canceladas.
2. **Médico**:
   - Possui login próprio focado na operação.
   - Analisa todos os agendamentos atribuídos ao seu nome e gerencia os seus pacientes no dia a dia.
3. **Administrador**:
   - Possui uma visão macro do negócio.
   - Pode cadastrar/aprovar novos médicos, revisar as contas dos pacientes e promover novos usuários como administradores.
   - Modifica dados gerais do sistema.

Além disso, a plataforma provê uma **API REST** para serviços de terceiros buscarem médicos (`GET /api/doctors`), sendo segura por um `Bearer Token`.

## 🛠️ Como rodar o projeto na sua máquina

Para executar o projeto, você precisará ter o [PHP](https://www.php.net/), e o [Composer](https://getcomposer.org/) instalados:

```bash
# Faça o clone
$ git clone https://github.com/SEU-USUARIO/MedMazza.git
$ cd MedMazza

# Preencha suas configurações do banco no .env
$ cp .env.example .env

# Instale os pacotes 
$ composer install
$ php artisan key:generate

# Execute as migrations e rode o sistema
$ php artisan migrate --seed
$ php artisan serve
```
