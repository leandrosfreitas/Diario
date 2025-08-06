# 📝 Diário Interativo - Projeto Django

Este é um projeto desenvolvido com Django 5.1 que permite criar e visualizar entradas de diário associadas a pessoas. Ideal para estudos de Django com foco em relacionamentos entre modelos, upload de imagens e uso de templates com Tailwind CSS.

## 🚀 Funcionalidades

- Cadastro de pessoas com foto
- Criação de entradas de diário (com título, texto e tags)
- Associação de pessoas às entradas
- Visualização das últimas entradas na página inicial
- Interface estilizada com Tailwind CSS

## 🛠 Tecnologias utilizadas

- [Python 3.12+](https://www.python.org/)
- [Django 5.1](https://www.djangoproject.com/)
- [Tailwind CSS](https://tailwindcss.com/)
- HTML5
- SQLite (padrão do Django)

## 📸 Tela inicial

> Página inicial exibindo os últimos 3 registros do diário:

![Exemplo de entrada do diário](media/foto/foto.png)

## 📂 Estrutura de diretórios (parcial)

```
core/
├── diario/
│   ├── models.py
│   ├── views.py
│   ├── urls.py
│   ├── templates/
│   │   ├── base.html
│   │   ├── home.html
│   │   ├── escrever.html
│   │   └── pessoa.html
├── media/
│   └── foto/
└── static/
```

## 🧪 Como rodar o projeto localmente

1. Clone o repositório:

```bash
git clone https://github.com/seu-usuario/diario-django.git
cd diario-django
```

2. Crie e ative um ambiente virtual:

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
```

3. Instale as dependências:

```bash
pip install -r requirements.txt
```

4. Execute as migrações:

```bash
python manage.py migrate
```

5. Inicie o servidor:

```bash
python manage.py runserver
```

6. Acesse em: [http://localhost:8000](http://localhost:8000)

## 🖼 Upload de Imagens

- As fotos cadastradas são salvas na pasta `media/foto/`
- Certifique-se de que `MEDIA_ROOT` e `MEDIA_URL` estão corretamente configurados em `settings.py`

## ✅ Próximas melhorias

- Paginação das entradas do diário
- Sistema de login/autenticação
- Edição e exclusão de registros
- Filtro por tags ou pessoas
  

---

> Projeto desenvolvido para fins educacionais.
