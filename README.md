# 🌐 Integração — Central de Serviços

Este projeto é uma aplicação web desenvolvida em **Python** com **Flask**, utilizando **Programação Orientada a Objetos (POO)** e integração a banco de dados MySQL através do **SQLAlchemy**.  
O objetivo é fornecer uma central de serviços que exibe informações em **combos, cards, tabelas e mapas interativos**, permitindo navegação dinâmica e organizada dos dados.

---

## 🚀 Funcionalidades

- **Interface Web com Flask**: rotas organizadas para diferentes componentes.
- **Banco de Dados MySQL**:
  - Conexão configurada via SQLAlchemy.
  - Automapeamento de tabelas existentes.
- **Combos Dinâmicos**:
  - Listagem de setores e locais.
  - Filtragem personalizada.
- **Cards de Serviços**:
  - Exibição de informações resumidas dos serviços.
- **Tabelas Dinâmicas**:
  - Visualização de serviços com diferentes estilos (básica, listrada, hover).
- **Mapa de Serviços**:
  - Representação visual dos locais e serviços disponíveis.

---

## 🛠️ Tecnologias Utilizadas

- **Backend**:
  - [Python 3.9+](https://www.python.org/)
  - [Flask](https://flask.palletsprojects.com/)
  - [SQLAlchemy](https://www.sqlalchemy.org/)
  - [mysql-connector-python](https://pypi.org/project/mysql-connector-python/)

- **Frontend**:
  - Templates HTML com [Jinja2](https://jinja.palletsprojects.com/)
  - Componentes customizados (combos, cards, tabelas, mapas).

- **Banco de Dados**:
  - MySQL (`db_central_servicos`).

---

## 📂 Estrutura do Projeto

Integracao-master/
│── main.py # Arquivo principal Flask (rotas)
│── models/ # Camada de modelos e integração com o banco
│ ├── db.py # Classe de conexão com MySQL
│ ├── model.py # Classe base para manipulação genérica de tabelas
│ ├── servico.py # Modelo de Serviços
│ ├── setor.py # Modelo de Setores
│ ├── local.py # Modelo de Locais
│ └── popular_*.py # Scripts para popular tabelas
│── opcoes/ # Componentes da aplicação
│ ├── cards.py # Geração de cards de serviços
│ ├── tabelas.py # Geração de tabelas de serviços
│ ├── combos.py # Geração de combos dinâmicos
│ └── mapa.py # Representação gráfica em mapa
│── integração/ # Arquivos auxiliares (modelos, imagens)
│ ├── CentralServicos.mwb # Modelo do banco (MySQL Workbench)
│ └── logo.jpg, loading.gif # Assets
│── templates/ # Páginas HTML (Flask + Jinja2)
│── static/ # Recursos estáticos (CSS, JS, imagens)

