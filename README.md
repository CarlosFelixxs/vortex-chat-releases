<div align="center">

# 🌀 Vortex Chat

### Voz, chat e compartilhamento de tela para jogar e conversar com amigos

[![Versão](https://img.shields.io/github/v/release/CarlosFelixxs/vortex-chat-releases?label=vers%C3%A3o&color=5865F2)](https://github.com/CarlosFelixxs/vortex-chat-releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/CarlosFelixxs/vortex-chat-releases/total?label=downloads&color=23A55A)](https://github.com/CarlosFelixxs/vortex-chat-releases/releases)
![Windows](https://img.shields.io/badge/plataforma-Windows-0078D4?logo=windows)

[**⬇️ Baixar a versão mais recente**](https://github.com/CarlosFelixxs/vortex-chat-releases/releases/latest)

</div>

---

## Sobre o Vortex

O **Vortex Chat** é um aplicativo privado de comunicação criado para reunir amigos em um único lugar. Ele oferece canais de texto e voz, chamadas em tempo real e compartilhamento de tela em alta qualidade.

Este repositório é o canal público e oficial de distribuição do aplicativo para Windows. Ele contém somente instaladores e arquivos necessários para atualização. O código-fonte e o desenvolvimento permanecem em um repositório privado.

Versão validada mais recente: **1.6.19**. O badge no topo e o link de download acompanham automaticamente as próximas releases públicas.

## Instalação

1. Abra a página da [versão mais recente](https://github.com/CarlosFelixxs/vortex-chat-releases/releases/latest).
2. Em **Assets**, baixe o arquivo `Vortex_Setup_X.Y.Z.exe`.
3. Execute o instalador e aguarde a conclusão.
4. Abra o Vortex pelo atalho criado no Windows.

> [!IMPORTANT]
> Baixe o Vortex somente por este repositório oficial. O instalador ainda não possui assinatura digital comercial, então o Windows pode exibir um aviso de editor desconhecido.

## Atualizações automáticas

A partir da versão **1.4.4**, instalações empacotadas do Vortex utilizam este repositório para receber atualizações. Na versão 1.6.19, o fluxo funciona assim:

- faz uma primeira verificação silenciosa depois da inicialização e repete aproximadamente a cada quatro horas;
- usa espera progressiva quando uma consulta falha, sem criar tentativas em loop;
- baixa em segundo plano somente fora de chamadas e compartilhamentos de tela;
- cancela e adia um download se uma atividade de voz ou tela começar;
- avisa quando a atualização está pronta;
- instala ao sair naturalmente do Vortex ou quando você escolher **Reiniciar agora**.

Assim, as próximas versões não precisam ser enviadas manualmente entre os usuários.

Builds de desenvolvimento, execução pelo navegador e pastas não empacotadas não usam o atualizador do Electron.

## Arquivos de cada versão

| Arquivo | Finalidade |
|---|---|
| `Vortex_Setup_X.Y.Z.exe` | Instalador oficial do aplicativo para Windows |
| `Vortex_Setup_X.Y.Z.exe.blockmap` | Permite downloads diferenciais e mais eficientes |
| `latest.yml` | Informa ao aplicativo a versão, tamanho e hash do instalador |

Os arquivos publicados recebem digests criptográficos do GitHub para ajudar na validação de integridade.

Para conferir manualmente o SHA-256 do instalador no PowerShell:

```powershell
Get-FileHash .\Vortex_Setup_1.6.19.exe -Algorithm SHA256
```

Compare o resultado com o digest mostrado pelo GitHub na mesma release. O `latest.yml` também contém tamanho e SHA-512 usados pelo atualizador.

## Requisitos

- Windows 10 ou Windows 11, 64 bits;
- conexão com a internet;
- microfone para chamadas de voz;
- permissão de captura para compartilhar a tela.

## Privacidade e acesso

O instalador é público para permitir atualizações automáticas sem expor credenciais. Isso **não torna público o código-fonte**, os pull requests, a documentação interna ou os segredos de infraestrutura do Vortex.

## Se a atualização não aparecer

1. confirme que a versão desejada está em [Releases](https://github.com/CarlosFelixxs/vortex-chat-releases/releases) e não como pré-lançamento;
2. use uma instalação do Vortex, não o ambiente local de desenvolvimento;
3. encerre chamadas e transmissões para liberar o download;
4. mantenha o aplicativo aberto por alguns minutos ou use a verificação manual disponível nas configurações;
5. confirme que GitHub não está bloqueado pela rede ou pelo antivírus;
6. se o pacote já foi baixado, feche e abra o Vortex para aplicar.

Problemas de segurança devem seguir [`SECURITY.md`](SECURITY.md), sem publicar tokens, dados pessoais ou detalhes sensíveis em issues.

---

<div align="center">

Feito para manter os amigos conectados. 💜

[Releases](https://github.com/CarlosFelixxs/vortex-chat-releases/releases) · [Última versão](https://github.com/CarlosFelixxs/vortex-chat-releases/releases/latest) · [Segurança](SECURITY.md)

</div>
