# Roadmap App

## Sobre o Projeto

O **Roadmap App** é uma plataforma para ajudar desenvolvedores a planejarem, acompanharem e documentarem seus projetos. O objetivo é manter a organização, registrar o progresso e facilitar o aprendizado durante o desenvolvimento.

## Tecnologias Utilizadas

- **Backend:** Django Rest Framework + MySQL
- **Frontend:** React + Tailwind CSS (futuro desenvolvimento)
- **Banco de Dados:** MySQL
- **Autenticação:** Django User Model

## Estrutura do Projeto

### Modelos de Dados

- **Usuários:** Gerenciados pelo Django User Model.
- **Roadmaps:** Representam os planos e objetivos do usuário.
- **Tarefas:** Passos dentro de um roadmap, com status (pendente, em andamento, concluída).
- **Documentação:** Notas e informações relacionadas a cada roadmap.

## Como Rodar o Projeto

### 1. Clonar o Repositório

```bash
git clone https://github.com/seu-usuario/roadmap-app.git
cd roadmap-app
```

### 2. Criar e Ativar um Ambiente Virtual

```bash
python -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate
```

### 3. Instalar as Dependências

```bash
pip install -r requirements.txt
```

### 4. Configurar o Banco de Dados

No arquivo `settings.py`, configure o MySQL:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'roadmap_db',
        'USER': 'seu_usuario',
        'PASSWORD': 'sua_senha',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

### 5. Rodar Migrações e Iniciar o Servidor

```bash
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
```

Acesse o backend em: `http://127.0.0.1:8000/`

---

## Próximos Passos

- Criar o frontend em React
- Implementar autenticação e autorização
- Adicionar um painel de controle para gerenciar roadmaps

---

Desenvolvido por Erik de Oliveira Freitas

