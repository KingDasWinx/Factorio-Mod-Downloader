# Factorio Mod Downloader
Uma ferramenta com interface gráfica para download automático de mods e suas dependências para o jogo Factorio.
![Exemplo da Interface](https://github.com/KingDasWinx/Factorio-Mod-Downloader/blob/main/image.png)

## Funcionalidades
- Interface gráfica amigável feita com CustomTkinter
- Download automático de mods e suas dependências
- Processamento paralelo para downloads mais rápidos
- Verifica versões compatíveis com Factorio 1.1
- Gerenciamento automático de dependências
- Log detalhado do processo de download
- Barra de progresso para acompanhamento
- Sistema de cache para evitar downloads duplicados

## Download e Instalação

### Versão Executável (Recomendado para usuários Windows)
1. Acesse a [página de Releases](https://github.com/KingDasWinx/Factorio-Mod-Downloader/releases)
2. Baixe a versão mais recente do arquivo `FactorioModDownloader.exe`
3. Execute o arquivo baixado - Não é necessária instalação

### Versão Python (Para desenvolvedores ou outros sistemas operacionais)

#### Pré-requisitos
```bash
Python 3.6+
```

#### Instalação
1. Clone este repositório:
```bash
git clone https://github.com/KingDasWinx/factorio-mod-downloader.git
```
2. Instale as dependências necessárias:
```bash
pip install customtkinter requests beautifulsoup4
```

## Como Usar
1. Execute o programa:
   - Versão .exe: Clique duas vezes no executável baixado
   - Versão Python: Execute `python index.py` no terminal
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
- Versão executável compilada com PyInstaller

## Contribuindo
Sinta-se à vontade para:
1. Abrir issues
2. Enviar Pull Requests
3. Sugerir melhorias
4. Reportar bugs

## Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.

## Autor
João Moreira - [KingDasWinx](https://github.com/KingDasWinx)
