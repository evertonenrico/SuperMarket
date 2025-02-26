# Super Market Sales
 Análise - Super Mercado

## Ferramentas Utilizadas

-Google Sheets;
-Google BigQuery;
-Power BI

## Contexto
O crescimento de supermercados nas cidades mais populosas está aumentando e a competição de mercado também é acirrada. 
O conjunto de dados analisado contém vendas históricas de uma rede de supermercados, registradas em 3 filiais diferentes durante 3 meses.
Métodos de análise preditiva de dados são fáceis de aplicar com este dataset.

## Início da Análise

O primeiro passo será analisar o arquivo que está no formato .CSV (separado por vírgulas) que nos foi enviado.
Abriremos o arquivo no *Google Sheets* para padronizar o nome das colunas, removendo espaços, caracteres especiais e erros.

A planilha será importada para o **Google BigQuery** para que possamos consultar os dados hospedados na nuvem.
Lembrando que neste momento,os dados não serão atualizados.

**Metadados**

ID da fatura: Número de identificação da nota fiscal gerado automaticamente
Filial: Unidade do supermercado (3 filiais disponíveis, identificadas por A, B e C)
Cidade: Localização das filiais
Tipo de cliente: Categoria do cliente ("Membro" para clientes com cartão fidelidade e "Normal" para sem cartão)
Gênero: Sexo do cliente (Masculino/Feminino)
Linha de produtos: Categorias de produtos:

 *Acessórios eletrônicos
 *Acessórios de moda
 *Alimentos e bebidas
 *Saúde e beleza
 *Casa e estilo de vida
 *Esportes e viagens

Preço unitário: Valor individual do produto em USD ($)
Quantidade: Número de produtos comprados
Imposto: Taxa de 5% aplicada sobre a compra
Total: Valor final incluindo impostos
Data: Data da compra (Registros de janeiro/2019 a março/2019)
Horário: Hora da compra (entre 10h e 21h)
Pagamento: Método utilizado (Dinheiro, Cartão de crédito ou Carteira digital)
CMV (Custo das Mercadorias Vendidas): Custo direto dos produtos
Percentual de margem bruta: Porcentagem da margem de lucro bruto
Renda bruta: Lucro bruto total
Avaliação: Classificação dada pelo cliente à experiência de compra (Escala de 1 a 10)

Observações:
Termos técnicos como Gross Margin Percentage e COGS mantêm suas siglas em inglês por convenção contábil, mas foram traduzidos entre parênteses.

"Ewallet" foi adaptado para "Carteira digital" (ex: PicPay, Mercado Pago).