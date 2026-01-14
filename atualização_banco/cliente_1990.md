## CLIENTE 1990

→ Executar blocos:
## RX
## ATENDIMENTO  
## CUSTO  
## FATURAMENTO  

## BANCO — 4

## RX — PRÉ-REQUISITO (caso não tenham rodado na rotina)
./ppa rxb -t atcabecatend
./ppa rxb -t ricadpac
./ppa rxb -t htatendimento
./ppa rxb -t  htpaciente

## ATENDIMENTO

 ./ppa dsb -s sghi/datasets/f_at_aten_interno__ricadint.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_aten_externo__recadate.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_aten_externo__reexcate.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_mov_paciente__rictrloc.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_leito_dia__sghdw.ds.yml
 ./ppa dsb -s sghi/datasets/fa_at_fluxo_atendimento__tbfluxoatend.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_pesquisa_satisfacao__scentrev.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_inatividade_leito__riinalei.ds.yml

# CUSTO

 ./ppa dsb -s sghi/datasets/f_at_exame__silanexa.ds.yml
 ./ppa dsb -s sghi/datasets/f_ct_custo__ctlancto.ds.yml
 ./ppa dsb -s sghi/datasets/f_ct_indicador__ctitepro.ds.yml

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