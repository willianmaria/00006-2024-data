# Contextualização

Conjunto de dados educacionais gerados de forma aleatória e com dados fictícios.

## Dicionário de dados

### alunos.csv

Dados dos alunos. Esta tabela contém informações pessoais sobre os alunos.

|Campo | Descrição |
|:--------:|------:|
| id | Identificador único do registro de pessoa do aluno |
| nome | Nome do aluno |
| data_nascimento | Data de nascimento do aluno |

### cursos.csv

Dados dos cursos. Esta tabela contém informações sobre os diferentes cursos oferecidos.

| Campo | Descrição |
|:--------:|------:|
| id | Identificador único |
| nome | Nome do curso |
| area_atuacao | Área de atuação do curso |

### disciplinas.csv

Dados das disciplinas. Esta tabela contém informações sobre as diferentes disciplinas oferecidas nos cursos.

| Campo | Descrição |
|:--------:|------:|
| id | Identificador único |
| nome | Nome da disciplina |
| sigla | Sigla da disciplina |
| dia_semana | Dia da semana que acontecem as aulas da disciplina (SEGUNDA = 0 ... DOMINGO = 6) |
| carga_horaria | Carga horária da disciplina |
| avaliacoes | Quantidade de avaliações da disciplina |

### turmas.csv

Dados das turmas. Esta tabela contém informações sobre as diferentes turmas formadas para cada curso.

| Campo | Descrição |
|:--------:|------:|
| id | Identificador único |
| id_curso | Código do curso da turma |
| nome | Nome da turma |
| data_inicio | Data de início da turma |
| data_termino | Data de término da turma |

### turma_avaliacoes.csv

Dados das avaliações das turmas. Esta tabela contém informações sobre as diferentes avaliações realizadas em cada turma.

| Campo | Descrição |
|:--------:|------:|
| titulo | Título da avaliação |
| id_turma | Código da turma |
| id_disciplina | Código da disciplina |
| data_avaliacao | Data de aplicação da avaliação |

### matriculas.csv

Dados das matrículas. Esta tabela contém informações sobre as matrículas dos alunos nas diferentes turmas.

| Campo | Descrição |
|:--------:|------:|
| id_matricula | Identificador único da Matrícula / Registro acadêmico |
| id_turma | Código da turma |
| id_aluno | Código do aluno (pessoa) |
| data_matricula | Data de realização da matrícula |
| situacao | Situação da matrícula |
| data_situacao | Data de atualização da situação da matrícula |

### matricula_disciplinas.csv

Dados das disciplinas cursadas nas matrículas. Esta tabela contém informações sobre as disciplinas que cada aluno está matriculado.

| Campo | Descrição |
|:--------:|------:|
| id_matricula | Código da matrícula |
| id_disciplina | Código da disciplina |

### matricula_aulas.csv

Dados das presenças nas aulas. Esta tabela contém informações sobre a presença dos alunos nas aulas.

| Campo | Descrição |
|:--------:|------:|
| id_matricula | Código da matrícula |
| id_disciplina | Código da disciplina |
| data_aula | Data de realização da aula |
| presente | Flag de presença do aluno |

### matricula_notas.csv

Dados das notas dos alunos. Esta tabela contém informações sobre as notas que os alunos receberam em suas avaliações.

| Campo | Descrição |
|:--------:|------:|
| id_matricula | Código da matrícula |
| id_disciplina | Código da disciplina |
| data | Data que a nota foi aplicada |
| nota | Nota do aluno na avaliação |
