Este repositório diz respeito à um web scrapper desenvolvido com o fim de obter informações do site da imobiliária Imperium Imóveis (https://www.imperiumimoveis.com.br/imoveis/venda-guarapuava).

Por se tratar de um site que utiliza rolagem infinita é necessário percorrer/carregar toda a página para ser ter acesso às informações.
O código efetua carregamentos na página até que o tamanho máximo da mesma seja atingido.

Além da rolagem infinita, esse site utiliza-se de estruturas diferentes para exibir os anúncios a depender de quais informações estão disponíveis no mesmo. Ou seja, caso o imóvel não possua preço anunciado, e sim "VALOR A CONSULTAR", o XPATH do elemento na página é diferente. Só para a informação de preço existem 3 possíveis XPATHs. As informações disponíveis nos anúncios não são padronizadas (ao mesmo tempo que o anúncio de uma casa pode mostrar além de áreas total e útil quantos quartos e banheiros a mesma possui, outro anúncio de casa pode informar apenas a quantidade de banheiros).

O código coleta um código de identificação do imóvel e o preço informado no site.
