# Atividade-Integrada-Grupo-04
Integrantes:
Caio marqs: https://github.com/Caio-Marq
Gabriel : https://github.com/GabrielB23hub
Deyvid Maciel: https://github.com/Deyvid333

TIGELA ROXA
ESTAREMOS VIRTUALIZANDO PEDIDOS DE AÇAÍ DA LOJA, TIGELA ROXA.
COMO ELES REALIZAM SUAS VENDAS:

Escopo do Projeto
O que está dentro do escopo:

Sistema web interno feito em Python com Streamlit e banco de dados SQLite, projetado para uso exclusivo em computadores (estações de trabalho Windows 10 e Linux Debian 13) na operação de açaiterias delivery (usando a Tigela Roxa como cliente piloto e modelo para futuras vendas ou locações a outras lojas).

Tela de login para os funcionários e administrador acessarem as funções do sistema.

Tela inicial (dashboard) mostrando o faturamento do dia e do mês (somando apenas pedidos entregues), o total de pedidos e os avisos de ingredientes com estoque baixo.

Cadastro e edição de preços e limites dos tamanhos de açaí (P de 300 g até 3 complementos, M de 500 g até 4, G de 1 kg até 5 e GG de 1,5 kg até 7) e dos complementos (porções de 50 g).

Tela para lançar pedidos feitos por telefone, permitindo montar o açaí manualmente ou escolher combos prontos, editar o pedido enquanto não estiver embalado (Pronto) e cancelar quando necessário.

Tela para a equipe de produção acompanhar a fila e atualizar o status dos pedidos (Aguardando, Em preparo, Pronto e Entregue).

Controle de estoque com baixa automática do açaí e dos complementos assim que o pedido entra em preparo, reposição manual em caso de cancelamento, histórico de movimentações e alerta de estoque mínimo configurado por ingrediente.

Cadastro de promoções acumuláveis (desconto em porcentagem para combos prontos e desconto direto no valor de itens específicos) com data de início e fim editáveis.

Histórico de vendas por período, relatório completo para a produção e opção de desativar registros em vez de apagar do banco de dados.

Landing Page comercial em HTML e CSS responsiva (para computador, tablet e celular) apresentando o sistema para outras açaiterias interessadas e liberando o download do código-fonte.

Configuração da rede local (roteador/AP com DHCP), três contêineres separados no servidor (DNS, Web e aplicação Python) e testes funcionando nas máquinas virtuais Windows 10 e Linux Debian 13.[RF_Sistema_Tigela_Roxa_v2.docx](https://github.com/user-attachments/files/35287044/RF_Sistema_Tigela_Roxa_v2.docx)

   

### Detalhamento do Objetivo

**Apresentação do Projeto**
O projeto consiste na criação de um sistema interno para gerenciar o delivery de açaiterias. Vamos usar a loja Tigela Roxa como primeiro cliente e exemplo prático na apresentação, mas a ideia é que o sistema também possa ser vendido ou alugado para outras açaiterias que trabalham da mesma forma. Como muitos computadores de pequenos comércios têm bloqueios que impedem instalar programas pesados ou bancos de dados externos, o sistema será feito em Python, usando Streamlit para as telas e SQLite para guardar os dados. Também faremos uma Landing Page em HTML e CSS para apresentar o sistema para outras lojas interessadas e liberar o download do código, tudo rodando em rede local com contêineres e DNS.

**Problema Identificado**
No dia a dia de uma açaiteria delivery como a Tigela Roxa, anotar pedidos de telefone no papel ou em planilhas soltas e controlar o estoque separado acaba gerando vários problemas:

* O atendente anota o pedido, mas a informação demora a chegar para quem está montando o açaí, atrasando a entrega.
* Sem baixar os ingredientes automaticamente a cada pedido, a loja só descobre que acabou açaí ou algum complemento quando o pote já está vazio.
* Somar complementos extras e calcular promoções diferentes no mesmo pedido de cabeça aumenta a chance de cobrar o valor errado do cliente.
* Sem um registro centralizado, o dono não consegue saber facilmente quanto faturou no dia, na semana ou no mês, nem conferir o que entrou e saiu do estoque.

**Objetivo Geral**
Desenvolver um sistema web leve em Python (com Streamlit e SQLite), rodando em rede local com contêineres, para controlar os pedidos, a fila de preparo, o estoque, as promoções e o faturamento de açaiterias — começando pela Tigela Roxa como cliente piloto, mas pronto para ser adaptado e vendido para outras lojas do mesmo ramo.

**Objetivos Específicos**

* Cadastrar os pedidos recebidos por telefone (com dados do cliente, forma de pagamento e observações), travando a quantidade de complementos conforme o tamanho escolhido (P até 3, M até 4, G até 5 e GG até 7) e permitindo editar o pedido antes de ele ser embalado.
* Criar uma tela para a equipe da cozinha acompanhar a fila de pedidos e mudar o status conforme o andamento (Aguardando, Em preparo, Pronto e Entregue), além de permitir cancelar pedidos quando precisar.
* Descontar automaticamente do estoque o peso do açaí (300 g, 500 g, 1 kg ou 1,5 kg) e os 50 g de cada complemento no momento em que o pedido entra em preparo, registrando o histórico de movimentação e avisando quando algum ingrediente atingir a quantidade mínima definida para ele.
* Calcular o valor final somando o preço do tamanho do açaí com os complementos, aplicando promoções acumuláveis (desconto em porcentagem para combos prontos e desconto direto em itens específicos) dentro das datas programadas.
* Mostrar na tela inicial quanto a loja faturou no dia, na semana e no mês (contando só os pedidos entregues), a quantidade de pedidos e os avisos de estoque baixo, além de gerar o relatório para a produção e o histórico de vendas.
* Usar a opção de desativar em vez de apagar produtos, ingredientes e promoções do banco de dados, para não perder o histórico dos relatórios antigos.
* Deixar os tamanhos, preços, ingredientes e promoções totalmente editáveis pelo administrador, facilitando a venda ou aluguel do sistema para outras açaiterias sem precisar mexer no código.
* Configurar a rede local com roteador/AP e DHCP, subir os contêineres de DNS, Web (Landing Page) e da aplicação Python no servidor, e testar tudo funcionando nos computadores Windows 10 e Linux Debian 13.
* 
# links dos protótipos
https://docs.google.com/document/d/1bockSs1NxKfq03jrBzip6TgETQ2Hat0MFk7Qs6IlLcE/edit?usp=sharing

# Repositorio da Landing Page
https://github.com/Deyvid333/Atividade-Integrada-Grupo04-Landing-page

# levantamentos de requiitos
# Software
* Requisitos funcionais
[[https://docs.google.com/document/d/1PlioxR3nxUemgb2hZsqcI2RViw1EgvuJ/edit](https://docs.google.com/document/d/1PlioxR3nxUemgb2hZsqcI2RViw1EgvuJ/edit?usp=sharing&ouid=118158459684752374556&rtpof=true&sd=true)](https://docs.google.com/document/d/1PlioxR3nxUemgb2hZsqcI2RViw1EgvuJ/edit?usp=sharing&ouid=118158459684752374556&rtpof=true&sd=true)
* Requisitos não funcionais
[https://docs.google.com/document/d/1ei88qu-jAL8vgZwMDTffz76qO3IF4_EF/edit?usp=sharing&ouid=118158459684752374556&rtpof=true&sd=true](https://docs.google.com/document/d/1ei88qu-jAL8vgZwMDTffz76qO3IF4_EF/edit?usp=sharing&ouid=118158459684752374556&rtpof=true&sd=true)
* Regras de Negócio
[https://docs.google.com/document/d/1JlpX4Bheyf8nH5ZLgDaBBCJUIlHeVkWT/edit](https://docs.google.com/document/d/1JlpX4Bheyf8nH5ZLgDaBBCJUIlHeVkWT/edit?usp=sharing&ouid=118158459684752374556&rtpof=true&sd=true)

# landingpage
* Requisitos funcionais
[https://docs.google.com/document/d/11lneZRuHjyKVcSoGDmfX9ewN5HGER13L/edit](https://docs.google.com/document/d/11lneZRuHjyKVcSoGDmfX9ewN5HGER13L/edit?usp=sharing&ouid=118158459684752374556&rtpof=true&sd=true)
* Requisitos não funcionais
https://docs.google.com/document/d/1V4H4OQufnczN5mXa3WiEXKg_7yAvvDVg/edit?usp=sharing&ouid=118158459684752374556&rtpof=true&sd=true
* Regras de Negócio
https://docs.google.com/document/d/1V4H4OQufnczN5mXa3WiEXKg_7yAvvDVg/edit

