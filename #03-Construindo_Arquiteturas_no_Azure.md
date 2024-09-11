# Grupo de Recursos

## Portal do Azure 

Faça login no [Portal do Azure](https://portal.azure.com).

## Criação do Grupo de Recursos

No painel do Azure, busque por “Grupos de Recursos” ou “Resource Groups” na barra de pesquisa.
Clique em **"Criar"** para iniciar a criação de um novo grupo de recursos.
Preencha as seguintes informações:
   - **Nome do Grupo de Recursos**: Dê um nome que identifique facilmente o grupo e seu propósito.
   - **Região**: Selecione a região onde o grupo será criado. É recomendado escolher a mesma região para todos os recursos relacionados para reduzir a latência e os custos.
Clique em **"Revisar + Criar"** e depois em **"Criar"**.

## Criação da Rede Virtual

No painel do Azure, busque por “Redes Virtuais” ou “Virtual Networks”.
Clique em **"Criar"** para iniciar a configuração de uma nova rede virtual.

Preencha os detalhes:
   - **Nome da Rede Virtual**: Escolha um nome que facilite a identificação da rede.
   - **Grupo de Recursos**: Selecione o grupo de recursos criado anteriormente.
   - **Região**: Escolha a mesma região do grupo de recursos.
   - **Endereço IP**: Defina o intervalo de endereços IP para a rede virtual.
  
   
Clique em **"Revisar + Criar"** e depois em **"Criar"**.

# Boa Prática em Segurança da Informação na Azure

## Criação de Regras no Grupo de Recursos

Para garantir a segurança e a eficiência dos seus recursos, é fundamental configurar regras apropriadas no Grupo de Recursos. Aqui está como você pode criar e gerenciar essas regras:

**Acesse o Grupo de Recursos**:
   - No painel do Azure, busque por “Grupos de Recursos” e selecione o grupo que você deseja configurar.

**Configuração de Regras de Segurança**:
   - **Grupo de Segurança de Rede (NSG)**: Adicione ou configure regras de segurança para controlar o tráfego de entrada e saída. No painel de NSG, você pode definir regras para permitir ou negar tráfego com base em IPs, portas e protocolos.
   - **Regras de Acesso**: Configure permissões e políticas para usuários e serviços que acessam o grupo de recursos. Utilize funções e permissões apropriadas para garantir que apenas usuários autorizados possam modificar ou visualizar os recursos.

**Monitoramento e Alertas**:
   - **Configuração de Alertas**: Defina alertas para monitorar atividades e possíveis violação de políticas de segurança. Configure notificações para ações suspeitas ou uso não autorizado de recursos. 

**Revisão e Atualização**:
   - **Revisão Periódica**: Realize revisões periódicas das regras e políticas para garantir que estejam atualizadas com as melhores práticas e os requisitos de segurança atuais.

## Exemplo de Vulnerabilidades com Falta de Regras em Grupo de Recursos

Caso você não crie regras apropriadas em um Grupo de Recursos, pode enfrentar as seguintes vulnerabilidades:

- **Acesso Não Controlado**: Recursos dentro do grupo podem ser acessados por usuários não autorizados, expondo dados sensíveis e comprometendo a segurança. 
- **Ataques de Rede**: Sem regras de segurança adequadas, suas redes podem estar suscetíveis a ataques externos, como DDoS ou acesso não autorizado a portas abertas. 
- **Custo Excessivo**: Recursos não monitorados podem ser utilizados de maneira inadequada, resultando em custos inesperados e elevados. 
- **Falta de Monitoramento**: A ausência de configuração apropriada pode levar à falta de visibilidade sobre o uso e estado dos recursos, dificultando a identificação de problemas e a realização de auditorias. 

Certifique-se de sempre definir regras de segurança e monitoramento apropriadas para proteger seus recursos e otimizar o gerenciamento de custos.
