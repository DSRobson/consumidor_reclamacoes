# Dicionário de Dados — Reclamações Anatel

## Fonte
Agência Nacional de Telecomunicações (Anatel)
https://dados.anatel.gov.br
Período: 2020 a fevereiro de 2026

---

## fReclamacoes (Tabela Fato)

| Coluna        | Descrição                                 |
|---------------|-------------------------------------------|
| id_reclamacao | Identificador único da reclamação         |
| data_abertura | Data em que a reclamação foi aberta       |
| id_empresa    | Chave para dEmpresa                       |
| id_assunto    | Chave para dAssunto                       |
| id_servico    | Chave para dServico                       |
| id_canal      | Chave para dCanal                         |
| id_estado     | Chave para dEstado                        |
| id_municipio  | Chave para dMunicipio                     |
| reaberta      | Se a reclamação foi reaberta (S/N)        |

---

## Tabelas Dimensão

### dEmpresa
| Coluna     | Descrição           |
|------------|---------------------|
| id_empresa | Chave primária      |
| empresa    | Nome da operadora   |

### dAssunto
| Coluna     | Descrição                           |
|------------|-------------------------------------|
| id_assunto | Chave primária                      |
| assunto    | Motivo da reclamação (ex: Cobrança) |

### dServico
| Coluna     | Descrição                         |
|------------|-----------------------------------|
| id_servico | Chave primária                    |
| servico    | Tipo de serviço (SMP, STFC, SeAC) |

### dCanal
| Coluna   | Descrição                              |
|----------|----------------------------------------|
| id_canal | Chave primária                         |
| canal    | Canal de entrada (Web, Call Center...) |

### dEstado
| Coluna    | Descrição       |
|-----------|-----------------|
| id_estado | Chave primária  |
| uf        | Sigla do estado |

### dMunicipio
| Coluna       | Descrição         |
|--------------|-------------------|
| id_municipio | Chave primária    |
| municipio    | Nome do município |
