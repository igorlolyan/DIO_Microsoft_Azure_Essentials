# Criando Máquinas Virtuais na Azure

## Acesse o Portal do Azure

Inicie acessando o portal do Azure e faça login para gerenciar seus recursos.

## Criando a VM

No painel do Azure, busque por “Máquinas Virtuais” ou “Virtual Machines” e clique em "Criar" para iniciar a configuração da sua VM.

## Preenchendo os Detalhes Básicos

- **Nome da VM**: Defina um nome que facilite a identificação da VM.
- **Região**: Escolha a região onde a VM será criada, preferencialmente próxima aos seus usuários.
- **Imagem**: Selecione o sistema operacional desejado, como Windows ou Linux.
- **Tamanho**: Determine o tamanho da VM conforme suas necessidades de CPU, memória e armazenamento.

## Configurando a Rede

- **Rede Virtual**: Crie ou selecione uma rede virtual existente.
- **Sub-rede**: Escolha a sub-rede para conectar a VM.
- **NSG (Network Security Group)**: Defina as regras de firewall que protegerão sua VM.

## Definindo as Credenciais

- **Usuário e Senha**: Configure as credenciais de login, certificando-se de usar uma senha forte e segura.

## Revisão e Criação

Revise todas as configurações e, se estiver tudo certo, clique em "Criar". O Azure levará alguns minutos para provisionar a VM.

## Conectando-se à VM

Assim que a VM for criada, conecte-se a ela. Para VMs Windows, use o Remote Desktop (RDP), e para VMs Linux, utilize o SSH.
