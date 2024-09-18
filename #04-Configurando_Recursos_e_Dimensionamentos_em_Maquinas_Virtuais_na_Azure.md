
# Configuração de Recursos e Dimensionamento em Máquinas Virtuais no Azure

## Passo a Passo para Criar Sua VM

### Acesse o Portal do Azure

Entre no [Portal do Azure](https://portal.azure.com).
No painel, procure por “Máquinas Virtuais” e clique em **"Criar"**. 


### Configure a Máquina Virtual

**Nome da VM**: Escolha um nome fácil de lembrar.

**Região**: Selecione a região mais próxima dos seus usuários para melhor desempenho.

**Imagem**: Escolha o sistema operacional (Windows ou Linux) que você deseja usar.

**Tamanho**: Selecione o tamanho da VM com base nas suas necessidades de CPU e memória.
   
### Configure o Dimensionamento da VM

**Dimensionamento Manual**: Escolha um tamanho de VM baseado na carga de trabalho esperada. O Azure oferece uma variedade de tamanhos de VM, desde opções básicas para tarefas leves até opções robustas para aplicações exigentes.

**Dimensionamento Automático**: Configure a autoescala para ajustar automaticamente os recursos da VM conforme a demanda. Isso é útil se você tem variações significativas no uso ou precisa garantir que a VM possa lidar com picos de carga. 
  
**Utilize o Azure Advisor**: O Azure Advisor fornece recomendações de dimensionamento com base no desempenho atual da sua VM. Ele pode sugerir ajustes para economizar custos ou melhorar o desempenho. 

### Configure a Rede

**Rede Virtual**: Crie uma nova rede ou escolha uma existente.
**Sub-rede**: Selecione a sub-rede para conectar sua VM.
**Grupo de Segurança de Rede (NSG)**: Defina regras para controlar o tráfego de entrada e saída da VM. Só permita o tráfego que você realmente precisa.

### Defina Credenciais

**Nome de Usuário e Senha**: Configure um usuário e senha fortes para acessar sua VM.
**Chaves SSH (para Linux)**: Se for Linux, use chaves SSH para se conectar com mais segurança.

### Configurações Adicionais

**Monitoramento**: Habilite o monitoramento para acompanhar o desempenho da VM.
**Tags**: Adicione tags para organizar melhor seus recursos.
   
### Revise e Crie

Revise todas as configurações.
Clique em **"Criar"** e aguarde enquanto o Azure prepara sua VM.
   
### Conecte-se à Sua VM

**Para Windows**: Use Remote Desktop (RDP) para se conectar.
**Para Linux**: Use SSH para acessar a VM.

# Cuidados Importantes para Produção

## **Segurança**

**Configuração do NSG**: Defina regras de firewall para proteger sua VM. Bloqueie tudo que não é necessário.
**Atualizações**: Mantenha o sistema e aplicativos atualizados.
**Gerenciamento de Credenciais**: Use senhas fortes e considere ferramentas como Azure Key Vault para gerenciar segredos.

## **Desempenho**

**Tamanho Adequado**: Escolha o tamanho certo da VM para evitar problemas de desempenho.
**Autoescala**: Configure o dimensionamento automático se sua carga de trabalho variar muito.

## **Backup**

**Backups Regulares**: Garanta que backups sejam feitos frequentemente.
**Plano de Recuperação**: Tenha um plano de recuperação em caso de falhas.

## **Monitoramento**

**Acompanhe o Desempenho**: Use ferramentas de monitoramento para verificar como a VM está funcionando.
**Relatórios**: Gere relatórios para ficar de olho no uso e na segurança.

## **Custo**

**Controle de Custos**: Acompanhe o uso e ajuste suas configurações para não gastar mais do que o necessário.
