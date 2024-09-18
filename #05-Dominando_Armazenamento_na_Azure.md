# Dominando o Armazenamento na Azure

## Passo a Passo para Configurar Armazenamento no Azure

### Acesse o Portal do Azure

Entre no [Portal do Azure](https://portal.azure.com).
No painel, procure por “Conta de Armazenamento” e clique em **"Criar"**.

### Configure a Conta de Armazenamento

**Nome da Conta**: Escolha um nome único para sua conta de armazenamento.

**Região**: Selecione a região mais próxima para melhor performance.

**Tipo de Conta**: Escolha "Armazenamento General Purpose v2".
  
**Replicação**: Selecione o tipo de replicação desejado (ex: LRS - Locally Redundant Storage).


### Criar um Compartilhamento de Arquivos 📁

**Acesse Sua Conta de Armazenamento**: No portal, vá para "Recursos" e selecione sua conta de armazenamento.
   
**Criar um Compartilhamento de Arquivos**: 
- No menu de "Serviços", clique em "Compartilhamento de Arquivos".
- Clique em "Adicionar compartilhamento de arquivos".
- Nomeie o compartilhamento e defina o tamanho.
- Clique em "Criar".
   
### Migrar Dados para o Azure

**Criar um projeto**: 
- Antes de tudo deve criar um projeto de migração para Azure:
     
**Instalar o AzCopy**: 
   - Baixe e instale o AzCopy do site oficial: [AzCopy Download](https://docs.microsoft.com/azure/storage/common/storage-use-azcopy-v10).

**Autenticar com o Azure**:
```bash
azcopy login
azcopy copy 'caminho/local/do/arquivo' 'https://<sua-conta>.file.core.windows.net/<compartilhamento>/<pasta>?<SAS-token>' --recursive
```
---
