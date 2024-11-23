# Factorio Mod Downloader

Uma ferramenta com interface gráfica para download automático de mods e suas dependências para o jogo Factorio.

![Exemplo da Interface](https://re146.dev/images/logo.png)

## Funcionalidades

- Interface gráfica amigável feita com CustomTkinter
- Download automático de mods e suas dependências
- Processamento paralelo para downloads mais rápidos
- Verifica versões compatíveis com Factorio 1.1
- Gerenciamento automático de dependências
- Log detalhado do processo de download
- Barra de progresso para acompanhamento
- Sistema de cache para evitar downloads duplicados

## Pré-requisitos

```bash
Python 3.6+
```

## Instalação

1. Clone este repositório:
```bash
git clone https://github.com/seu-usuario/factorio-mod-downloader.git
```

2. Instale as dependências necessárias:
```bash
pip install customtkinter requests beautifulsoup4
```

## Como Usar

1. Execute o script:
```bash
python index.py
```

2. Na interface gráfica que aparecer:
   - Cole a URL do mod do Factorio (formato: https://mods.factorio.com/mod/nome-do-mod)
   - Clique em "Baixar ModPack"
   - Aguarde o processo de download

3. Os mods serão baixados para:
   - Windows: `C:\Users\SeuUsuario\Downloads\FactorioMods`
   - Linux/Mac: `~/Downloads/FactorioMods`

## Estrutura do Projeto

```
factorio-mod-downloader/
│
├── index.py          # Arquivo principal com GUI e lógica de download
├── README.md         # Este arquivo
└── requirements.txt  # Dependências do projeto
```

## Como Funciona

O programa realiza as seguintes etapas:

1. Analisa a URL do mod fornecida
2. Busca todas as dependências recursivamente
3. Verifica as versões compatíveis com Factorio 1.1
4. Realiza o download paralelo dos mods e dependências
5. Salva os arquivos na pasta de downloads
6. Mantém um registro dos mods baixados para evitar duplicatas

## Recursos Técnicos

- Utiliza threading para downloads paralelos
- Cache de mods baixados em JSON
- Gestão automática de sessões HTTP
- Tratamento de erros robusto
- Interface responsiva durante downloads

## Contribuindo

Sinta-se à vontade para:
1. Abrir issues
2. Enviar Pull Requests
3. Sugerir melhorias
4. Reportar bugs

## Licença

Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

## Autor

Seu Nome - [Seu GitHub](https://github.com/seu-usuario)
