## CLIENTE 0103

→ Executar blocos:
## RX
## CUSTO  
## FINANCEIRO  
## FATURAMENTO  

## BANCO — 2


**NÃO HÁ NECESSIDADE DE TODAS AS TABELAS**


## RX — PRÉ-REQUISITO (caso não tenham rodado na rotina)
./ppa rxb -t atcabecatend
./ppa rxb -t ricadpac
./ppa rxb -t htatendimento
./ppa rxb -t  htpaciente

## CUSTO

./ppa dsb -s sghi/datasets/f_at_exame__silanexa.ds.yml
./ppa dsb -s sghi/datasets/f_ct_custo__ctlancto.ds.yml
./ppa dsb -s sghi/datasets/f_ct_indicador__ctitepro.ds.yml

## FINANCEIRO

 ./ppa dsb -s sghi/datasets/f_fi_movimento__mfconpag.ds.yml
 ./ppa dsb -s sghi/datasets/f_fi_movimento__mfctarec.ds.yml
 ./ppa dsb -s sghi/datasets/f_fi_movimento__mflancto.ds.yml
 ./ppa dsb -s sghi/datasets/f_fi_movimento__mfadifor.ds.yml
 ./ppa dsb -s sghi/datasets/f_fi_conta_saldo_dia__mflancto.ds.yml

## FATURAMENTO

 ./ppa dsb -s sghi/datasets/f_ft_item_faturado__falansus.ds.yml
 ./ppa dsb -s sghi/datasets/f_ft_item_faturado__fhlancto.ds.yml
 ./ppa dsb -s sghi/datasets/f_ft_item_faturado__fhcondia.ds.yml
 ./ppa dsb -s sghi/datasets/f_ft_item_faturado.ds.yml
 ./ppa dsb -s sghi/datasets/f_ft_item_faturado^udn2.ds.yml
 ./ppa dsb -s sghi/datasets/d_dados_faturamento__factasus.ds.yml
 ./ppa dsb -s sghi/datasets/d_dados_faturamento__fclanext.ds.yml
 ./ppa dsb -s sghi/datasets/d_dados_faturamento__fhcadaih.ds.yml
 ./ppa dsb -s sghi/datasets/f_ft_sus_paulista.ds.yml
 