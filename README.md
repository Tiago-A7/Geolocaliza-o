# Sistema de Geolocalização de Locais

![PHP](https://img.shields.io/badge/PHP-8.0+-777BB4?style=flat-square&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-5.7+-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5.3-7952B3?style=flat-square&logo=bootstrap&logoColor=white)
![Leaflet](https://img.shields.io/badge/Leaflet-1.9-199900?style=flat-square&logo=leaflet&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green.svg)

> Aplicação web para gestão e visualização de locais georreferenciados em mapa interativo, desenvolvida como projeto académico.

---

## 📋 Descrição do Projeto

Sistema completo de geolocalização que permite registar, visualizar e gerir locais de interesse (hospitais, aeroportos, hotéis, restaurantes, museus, etc.) num mapa interativo. Inclui autenticação de utilizadores, permissões diferenciadas, upload de fotografias e envio de informação por email.

O projeto foi desenvolvido com arquitetura **MVC simplificada**, separando claramente a lógica de apresentação (frontend), processamento (backend) e persistência de dados (base de dados).

---

## ✨ Funcionalidades Implementadas

### Funcionalidades Obrigatórias

| Funcionalidade | Descrição |
|----------------|-----------|
| 🔐 **Sistema de Login** | Autenticação segura com sessões PHP e hash SHA3-256 |
| 👥 **Tipos de Utilizadores** | Administrador (acesso total) e Utilizador Normal (apenas seus locais) |
| 🗺️ **Mapa Interativo** | Visualização com Leaflet, múltiplas camadas (OSM, Satélite, Terreno) |
| 📍 **Marcadores Georreferenciados** | Clique no mapa para definir coordenadas com reverse geocoding |
| 📝 **Formulário de Locais** | Inserção/edição com nome, categoria, morada, contactos e descrição |
| 🔍 **Pesquisa Avançada** | Filtros por país, cidade e categoria com paginação |
| 📊 **Menu Lateral** | Interface responsiva com navegação intuitiva |

### Funcionalidades Opcionais (Extras)

| Funcionalidade | Descrição |
|----------------|-----------|
| 📧 **Envio por Email** | Partilha de informação de locais via email com template HTML |
| 🖼️ **Upload de Fotografias** | Upload com validação (máx. 2MB), redimensionamento automático e preview |
| 📱 **Design Responsivo** | Adaptável a desktop, tablet e mobile |
| 🎨 **Categorias Personalizáveis** | Cores, siglas e ícones configuráveis por categoria |
| 📍 **Geolocalização do Utilizador** | Botão "Minha Localização" usando API do navegador |
| 🗑️ **Soft Delete** | Locais marcados como inativos em vez de apagados fisicamente |
| 🔔 **Notificações Toast** | Feedback visual em vez de alerts JavaScript |

---

## 🛠️ Tecnologias Utilizadas

### Backend
- **PHP 8.0+** - Linguagem de programação servidor
- **MySQL 5.7+** - Sistema de gestão de base de dados
- **PDO** - Interface de acesso à base de dados (prepared statements)

### Frontend
- **HTML5** - Estrutura semântica
- **CSS3** - Estilização personalizada
- **JavaScript (ES6+)** - Lógica de cliente
- **Bootstrap 5.3** - Framework CSS para interface responsiva
- **Bootstrap Icons** - Biblioteca de ícones

### Bibliotecas e APIs
- **Leaflet 1.9** - Biblioteca de mapas interativos
- **Leaflet.markercluster** - Agrupamento de marcadores
- **Nominatim (OpenStreetMap)** - Reverse geocoding (coordenadas → morada)

### Ferramentas de Desenvolvimento
- **XAMPP/WAMP/MAMP** - Ambiente de desenvolvimento local
- **Git** - Controlo de versões
- **Doxygen** - Documentação do código

---

## 🚀 Instruções para Executar o Projeto Localmente

### Pré-requisitos

- [XAMPP](https://www.apachefriends.org/) (Windows/Linux/Mac) ou similar (WAMP, MAMP)
- Navegador web moderno (Chrome, Firefox, Edge)
- Git (opcional, para clonar o repositório)

### Passo 1: Clonar o Repositório

```bash
# Usando HTTPS
git clone https://github.com/teu-utilizador/sistema-geolocalizacao.git

# Ou fazer download do ZIP e extrair
