# SIMULADO-PR-TICO-SISTEMAS-DISTRIBU-DOSS

Simulado Prático — Sistemas Distribuídos
Curso: Análise e Desenvolvimento de Sistemas
Professora: Prof.ª Dr.ª Simone Tatiane do Canto
Linguagem: Python
Ambiente: Visual Studio Code (VS Code)

Sobre o projeto
Este projeto foi desenvolvido como atividade prática da disciplina de Sistemas Distribuídos.

O objetivo é simular uma Central de Pedidos Distribuída, utilizando um servidor principal e uma réplica para demonstrar conceitos importantes de sistemas distribuídos.

Funcionalidades implementadas
Controle de concorrência: utilização de Semaphore para limitar o processamento a dois pedidos simultâneos.
Sincronização de dados: atualização do estoque da réplica conforme o estoque do servidor principal.
Tolerância a falhas: utilização da réplica quando o servidor principal fica indisponível.
Controle de acesso: utilização de Lock para evitar condições de corrida durante a atualização do estoque.
Tecnologias utilizadas
Python 3
Threading
Time
Visual Studio Code
Git e GitHub
Como executar o projeto
Clone este repositório.
Abra a pasta do projeto no VS Code.
Abra o terminal.
Execute o comando:

bash
python central_pedidos.py
Caso necessário, utilize:


bash
py central_pedidos.py
Resultado esperado

text
=== CENTRAL DE PEDIDOS ===
Limite simultâneo: 2
Estoque inicial: 10
Pedidos confirmados: [101, 102, 103]
Estoque principal: 7
Réplica antes: 10
Réplica depois: 7
Consulta após falha: REPLICA 7
Estrutura do projeto

text
simulado_distribuidos/
│
├── central_pedidos.py
└── README.md
Conceitos estudados
Concorrência
Threads
Semáforos
Locks
Replicação de dados
Consistência
Tolerância a falhas
Failover
Conclusão
A atividade permitiu compreender, na prática, como funcionam mecanismos de concorrência, sincronização de dados e tolerância a falhas em sistemas distribuídos, utilizando Python.
