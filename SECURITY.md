# Segurança dos downloads do Vortex

## Versões suportadas

A release pública mais recente recebe correções e validação completas. A versão anterior permanece disponível para rollback, mas usuários devem atualizar assim que a versão mais recente for aprovada.

## Origem oficial

Baixe o Vortex somente em:

`https://github.com/CarlosFelixxs/vortex-chat-releases/releases`

Cada versão válida contém exatamente:

- `Vortex_Setup_X.Y.Z.exe`;
- `Vortex_Setup_X.Y.Z.exe.blockmap`;
- `latest.yml`.

O workflow de publicação verifica presença, tamanho, estado de upload e digest SHA-256 dos três arquivos antes de tornar a release pública. O atualizador usa também o tamanho e o SHA-512 registrados em `latest.yml`.

O instalador ainda não possui certificado comercial de assinatura de código. Um aviso de editor desconhecido pode aparecer no Windows; isso não substitui a conferência da URL e do hash.

## Relatar uma vulnerabilidade

Não publique tokens, credenciais, dados pessoais, endereços IP, conteúdo de conversas ou instruções de exploração em uma issue pública.

Use uma [denúncia privada de segurança](https://github.com/CarlosFelixxs/vortex-chat-releases/security/advisories/new) e informe:

- versão afetada;
- comportamento observado;
- impacto provável;
- passos mínimos para reprodução;
- hashes ou nomes dos arquivos envolvidos, sem anexar segredos.

Suspeitas de instalador adulterado, atualização apontando para versão incorreta ou vazamento de credenciais devem ser tratadas como prioridade alta.

