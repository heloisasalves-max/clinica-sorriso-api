# Sorriso Metálico

Esse site foi solicitado por Dr. Roberto Carlos de Alencar. E é destinado a uma clínica que quer trazer uma esperiência Premium para seus cliente. Esse site deve conter login do cliente, agendamento de consultas com escolha de dentista, data e horário e identificação e marcação de clientes na categoria VIP.

## Mer
### cliente
- id_cliente PK
- senha VARCHAR(200)
- nome VARCHAR(150)
- cpf CHAR(11)
- vip BOOLEAN

### dentista
- id_dentista PK
- nome VARCHAR(150)
- especialidade VARCHAR(100)

### agendamento
- id_agendamento PK
- id_cliente FK
- id_dentista FK
- data_atendimento DATE
- horario_atendimento TIME
- status VARCHAR(30)

### relacionamento
- 1 cliente para varios agendamentos
- 1 dentista para varios agendamentos
## Der
![Diagrama der](./database/diagrama-clinica.drawio.png.)
