# Churn Rate Project
Projeto criado com a intenção de gerar insights diagnósticos sobre as motivações envolvidas na crescente taxa de cancelamento de serviços de uma empresa de streaming por assinatura. Segundo a diretoria, **a maior parte da sua base de clientes é formada por clientes que cancelaram o serviço**, ou seja, inativos. Com o intuito de **melhorar seus resultados e promover mudanças na promoção de seus serviços**, o objetivo do presente estudo é levantar os principais motivos dos cancelamentos e quais as possíveis ações para reduzir tal taxa.
<br/><br/>
Para tanto, os seguintes passos listados abaixo foram adotados:
1) Importação da base de dados
   <br/>
2) Visualização da base de dados
   <br/>
3) Tratamento de erros
   <br/>
5) Análise inicial dos dados para compreender o estado atual dos cancelamentos
   <br/>
6) Análise profunda dos dados para encontrar as motivações do cancelamento
   <br/>
  
Com a lista de passos em mãos, o desenvolvimento do código seguiu o seguinte raciocínio:
   <br/>
  I) importação das bibliotecas necessárias para a análise:  Matplotlib, Pandas, Seaborn e NumPy
   <br/>
 II) leitura do arquivo
<br/>
 III) visualização da tabela
<br/>
 IV) identificação e remoção de valores vazios
<br/>
 V) retirada de colunas desnecessárias
<br/>
 VI) análise da quantidade de pessoas que <b>cancelaram e não cancelaram (56,71% e 43,29%</b>, respectivamente)
<br/>
 VII) análise da quantidade de contratos por duração, em que nota-se que há uma <b>menor quantidade de contratos mensais (19,8%)</b>
<br/>
 VIII) ao realizar um agrupamentos dos contratos, observa-se que que a <b>média de cancelamentos na opção de contrato mensal é de 100%</b>, ou seja, todos cancelaram 
<br/>
 IX) <b>retirada da opção de contrato mensal</b> para observação de como os demais fatores se comportam. Como resultado, houve uma **queda a 46,1% dos cancelamentos**, que ainda é uma taxa alta
<br/>
 X) visualização gráfica dos demais fatores em relação ao cancelamento
<br/>
 XI) tipo de assinatura, gênero, idade, tempo como cliente e gasto total, à princípio, **parecem não ser fatores diretamente conectados a alta na taxa de cancelamentos**
<br/>
 XII) **ligação ao callcenter, tipo de contrato e número de dias de atraso no pagamento são fatores fortemente relacionados à taxa de cancelamento** da seguinte forma:
- tipo de contrato mensal, em média, 100% cancelou <br/>
- mais do que 5 ligações ao callcenter, em média, 100% cancelou<br/>
- mais do que 20 dias de atraso, em média, 100% cancelou<br/>

Com tais resultados, portanto, **sugerem-se as seguintes medidas**:<br/>
I) **Retirada de assinatura mensal**<br/>
II) **Contato com o cliente antes de chegar a 20 dias de atraso, buscando uma negociação ao pagamento em atraso**<br/>
III) **Oferecimento de desconto ao cliente que ligar 3/4 vezes ao callcenter**<br/>   

Assim, com a retirada dos fatores-problema citados anteriormente, **a taxa de cancelamento cai a 18,40%**, podendo ser mais ainda reduzida com a manipulação mais detalhada dos dados fornecidos. Por fim, o presente projeto conseguiu unir análises de forma descritiva, prescritiva e diagnóstica.

 
