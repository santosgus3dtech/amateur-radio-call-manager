# Estado atual do gerenciador de chamadas

Revisão: 13/10/2026. Git inicial limpo. Última etapa comprovada: inspeção documental e estática. Nenhum registro de chamada, banco ou exportação real foi aberto.

## Arquitetura e regras observadas

[main.py](../main.py) usa PyQt5, SQLite e bibliotecas de planilha. Cria a tabela `cadastro_chamadas` com identificador e campos de contato, data, horários, faixa/frequência, modo, sinais, confirmação e anotações. Há funções `inserir_dados`, `excluir_linha`, `atualizar_db` e `gerar_excel`. O [README](../README.md) descreve CRUD e atualização da tabela após alterações. Esse comportamento está documentado e há funções correspondentes; execução não foi verificada.

As telas `.ui` e módulos `ui_*.py` coexistem. [requirements.txt](../requirements.txt) inclui também `mysql-connector-python` e `colorama`; imports adicionais não demonstram integração MySQL ativa. Validação dos formulários e limites de exportação não foram conferidos funcionalmente.

## Operação e fontes

Consultar o [README](../README.md) para ambiente virtual, `pip install -r requirements.txt` e `python main.py`. Todos: **não executado nesta tarefa**. [Gerenciador.spec](../Gerenciador.spec) existe; não foi identificado comando repetível de build no README nem comando de teste. Não há certificação de execução ou empacotamento.

## Roadmap documentado e retomada

O README lista como próximas melhorias: empacotamento repetível, validação de formulário mais forte, testes das operações de banco e revisão de espaçamento/erros da UI. São propostas da documentação existente, sem evidência de aprovação, implementação ou conclusão nesta revisão. Não se criaram decisões históricas.

Sugestões de retomada, não compromissos aprovados: (1) confirmar quais dessas melhorias continuam desejadas; (2) verificar fluxo com banco sintético quando autorizado; (3) estabelecer uma verificação repetível de exportação/CRUD. A presente tarefa apenas preparou as notas.

[Índice](INDEX.md).
