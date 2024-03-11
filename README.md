# API Django REST Alunos List

Esta é uma API construída com Django REST Framework para gerenciar alunos, cursos e matrículas em uma escola.

## Instalação

1.Clone este repositório:

```bash
git clone https://github.com/ELIEZERBITTENCOURT/api-escola.git
```

2.Instale as dependências:

```bash
pip install -r requirements.txt
```

3.Execute as migrações do banco de dados:

```bash
python manage.py migrate
```

4.Inicie o servidor:

```bash
python manage.py runserver
```

A API estará acessível em `http://localhost:8000/`.

## Endpoints

- `admin/`: Painel de administração Django.
- `alunos/`: Lista de todos os alunos.
- `alunos/<int:pk>/`: Detalhes de um aluno específico.
- `cursos/`: Lista de todos os cursos.
- `cursos/<int:pk>/`: Detalhes de um curso específico.
- `matriculas/`: Lista de todas as matrículas.
- `matriculas/<int:pk>/`: Detalhes de uma matrícula específica.
- `aluno/<int:pk>/matriculas/`: Lista de matrículas de um aluno específico.
- `curso/<int:pk>/matriculas/`: Lista de alunos matriculados em um curso específico.

## Utilização

- `GET /alunos/`: Retorna uma lista de todos os alunos.
- `POST /alunos/`: Cria um novo aluno.
- `GET /alunos/<int:pk>/`: Retorna detalhes de um aluno específico.
- `PUT /alunos/<int:pk>/`: Atualiza os detalhes de um aluno específico.
- `DELETE /alunos/<int:pk>/`: Remove um aluno específico.
- Endpoint semelhante para cursos e matrículas.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir problemas (issues) e enviar pull requests para melhorar esta API.

## Licença

Este projeto é licenciado sob a [Licença MIT](https://opensource.org/licenses/MIT).
