⚡ SESI - Rastreamento de Consumo e Desperdício de Energia

SESI - Sistema de Rastreamento de Consumo e Desperdício de Energia

🧪 Testes com Thunder Client

Print:

prints/01_get_todos.png

Teste 2 - GET por ID
GET http://localhost:3000/equipamentos/1


Print:

prints/02_get_id.png

Teste 3 - Busca por equipamento
GET http://localhost:3000/buscar/equipamento/ar-condicionado


Print:

prints/03_busca_equipamento.png

Teste 4 - Busca por local
GET http://localhost:3000/buscar/local/laboratório


Print:

prints/04_busca_local.png

Teste 5 - POST
POST http://localhost:3000/equipamentos


Print:

prints/05_post_cadastro.png

Teste 6 - PUT
PUT http://localhost:3000/equipamentos/1


Print:

prints/06_put_atualizacao.png

Teste 7 - DELETE
DELETE http://localhost:3000/equipamentos/5



📊 Exemplo de dados

O arquivo dados.json contém registros semelhantes aos seguintes:

[
  {
    "id": 1,
    "local": "Laboratório 03",
    "equipamento": "Ar-condicionado",
    "consumo_kwh": 185.4,
    "mes_referencia": "2026-09",
    "status": "Consumo elevado"
  },
  {
    "id": 2,
    "local": "Sala 12",
    "equipamento": "Computadores",
    "consumo_kwh": 92.7,
    "mes_referencia": "2026-09",
    "status": "Consumo normal"
  },
  {
    "id": 3,
    "local": "Oficina Mecânica",
    "equipamento": "Compressor de ar",
    "consumo_kwh": 245.8,
    "mes_referencia": "2026-09",
    "status": "Consumo elevado"
  },
  {
    "id": 4,
    "local": "Biblioteca",
    "equipamento": "Iluminação",
    "consumo_kwh": 68.3,
    "mes_referencia": "2026-09",
    "status": "Consumo normal"
  },
  {
    "id": 5,
    "local": "Sala dos Professores",
    "equipamento": "Geladeira",
    "consumo_kwh": 54.6,
    "mes_referencia": "2026-09",
    "status": "Consumo normal"
  }
]

📋 Campos dos registros
Campo	Descrição
id	Identificador único do equipamento
local	Local onde o equipamento está instalado
equipamento	Nome do equipamento
consumo_kwh	Consumo de energia em kWh
mes_referencia	Mês utilizado como referência
status	Situação do consumo

⚠️ Validações

O sistema verifica se os campos obrigatórios foram preenchidos no cadastro.
Os campos obrigatórios são:

Local;
Equipamento;
Consumo em kWh;
Mês de referência;
Status.
Caso algum campo esteja vazio, a API retorna uma mensagem de erro.