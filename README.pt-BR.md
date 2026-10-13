# Amateur Radio Call Manager

[English / README principal](README.md) · Português (Brasil)

Aplicativo desktop desenvolvido para um radioamador registrar, editar, excluir e exportar registros de contatos de rádio.

O projeto surgiu de uma solicitação real do meu professor da faculdade, Virgilio Cesar Leandro. O objetivo era substituir o acompanhamento feito apenas em planilhas por um pequeno aplicativo local com interface gráfica e SQLite.

## O que demonstra

- Interface desktop em Python com PyQt5.
- Persistência com SQLite.
- Operações CRUD para registros de contatos.
- Atualização da tabela após inserções, alterações e exclusões.
- Exportação para Excel para compartilhamento e backup.

## Tecnologias

- Python
- PyQt5
- SQLite
- pandas
- openpyxl
- xlwt

## Estrutura do projeto

```text
amateur_radiocall_manager/
  main.py
  *.ui
  ui_*.py
  Gerenciador.spec
  requirements.txt
  README.md
```

## Instalação

```bash
python -m venv .venv
.venv/Scripts/activate
pip install -r requirements.txt
python main.py
```

O banco de dados SQLite local é criado durante a execução e é intencionalmente ignorado pelo Git.

## Funcionalidades

- Adicionar registros de contatos com data, hora, frequência e observações.
- Editar registros existentes.
- Excluir registros por ID.
- Exportar a tabela para um arquivo Excel.
- Manter a tabela da interface atualizada após alterações.

## Capturas de tela

![Tela principal](https://user-images.githubusercontent.com/113928099/228587507-17bb354d-e412-49f4-812c-dd4de65f9b79.png)
![Tela de inserção](https://user-images.githubusercontent.com/113928099/228587599-5790fa37-e634-43b4-9731-7a41c96b9417.png)
![Tela da tabela](https://user-images.githubusercontent.com/113928099/228587941-b570c1ff-aeab-4593-846f-9f12041605b1.png)

## Próximas melhorias

- Empacotar o aplicativo com um comando de build reproduzível.
- Adicionar uma validação mais rigorosa dos formulários.
- Adicionar testes automatizados para operações do banco de dados.
- Melhorar o espaçamento da interface e as mensagens de erro.
