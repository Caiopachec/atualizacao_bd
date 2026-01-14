## CLIENTE 0682

→ Executar blocos, em ordem:
## RX 
## ATENDIMENTO  
## AGENDA  
## CUSTO  
## FINANCEIRO  
## FATURAMENTO  
## SUPRIMENTOS    
## CUSTOMIZADOS
## PEP  

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

## AGENDA

./ppa dsb -s sghi/datasets/f_at_agendamento__repacagd.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_agendamento__sipacagi.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_cirurgia__cclancir.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_cirurgia_agendada__ccagenda.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_cirurgia_agendada__cchisage.ds.yml
 ./ppa dsb -s sghi/datasets/d_dados_cirurgia__cccadcir.ds.yml
 ./ppa dsb -s sghi/datasets/d_dados_parto__ccficpar.ds.yml

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

## SUPRIMENTOS / ESTOQUE

 ./ppa dsb -s sghi/datasets/f_sp_mov_produto__gelansai.ds.yml
 ./ppa dsb -s sghi/datasets/f_sp_mov_produto__gelandev.ds.yml
 ./ppa dsb -s sghi/datasets/f_sp_mov_produto__gelansaiopme.ds.yml
 ./ppa dsb -s sghi/datasets/f_sp_mov_produto__gelandevopme.ds.yml
 ./ppa dsb -s sghi/datasets/f_sp_compra__gelannfs.ds.yml
 ./ppa dsb -s sghi/datasets/f_sp_saldo_estoque_dia__gesaldos.ds.yml
 ./ppa dsb -s sghi/datasets/f_sp_saldo_estoque_mes__sghdw.ds.yml
 ./ppa dsb -s sghi/datasets/f_sp_pedido_compra__gelanped.ds.yml
 ./ppa dsb -s sghi/datasets/fa_sp_consumo.ds.yml

## CUSTOMIZADOS

 ./ppa dsb -s sghi/datasets/f_integra_bi.ds.yml
 ./ppa dsb -s sghi/datasets/f_rpa__rplaneve.ds.yml
 ./ppa dsb -s sghi/datasets/f_fp_resumo_folha2__fpfichaf.ds.yml
 ./ppa dsb -s sghi/datasets/bt_cdc_movimento__mfctarec.ds.yml
 ./ppa dsb -s sghi/datasets/bt_cdc_movimento__mfconpag.ds.yml
 ./ppa dsb -s sghi/datasets/bt_cdc_movimento__falansus.ds.yml
 ./ppa dsb -s sghi/datasets/bt_cdc_movimento__fclanext.ds.yml
 ./ppa dsb -s sghi/datasets/bt_cdc_movimento__rpa.ds.yml
 ./ppa dsb -s sghi/datasets/d_ag_cdc_movimento__mfconpag.ds.yml
 ./ppa dsb -s sghi/datasets/d_ag_cdc_movimento__mfctarec.ds.yml
 ./ppa dsb -s sghi/datasets/mat_view__d_item_cobr_mat_med__tbmatmed.ds.yml
 ./ppa dsb -s sghi/datasets/st_mfconpag_fav_cre__mfconpag.ds.yml
 ./ppa dsb -s sghi/datasets/vd_conta_hospitalar__sghdw.ds.yml
 ./ppa dsb -s sghi/datasets/10_st_class_risco_aten_externo.ds.yml
 ./ppa dsb -s sghi/datasets/10_st_enumerations.ds.yml
 ./ppa dsb -s sghi/datasets/20_atcabecatend__ex.ds.yml
 ./ppa dsb -s sghi/datasets/20_fcrefund__ex.ds.yml
 ./ppa dsb -s sghi/datasets/20_gecadsai__ex.ds.yml
 ./ppa dsb -s sghi/datasets/20_gelannfs__ex.ds.yml
 ./ppa dsb -s sghi/datasets/20_tbfluxoatend__ex.ds.yml
 ./ppa dsb -s sghi/datasets/20_tbmatmed__ex.ds.yml
 ./ppa dsb -s sghi/datasets/20_tbvlrmem__ex.ds.yml


## PEP (ORDEM OBRIGATÓRIA)
1. ./ppa dsb -s sghi/datasets/fl_pep_tmp__prevolpac.ds.yml
2. ./ppa dsb -s sghi/datasets/fl_pep_st_evolucoes__prevolpac.ds.yml
3. ./ppa dsb -s sghi/datasets/fl_pep_uevolucoes__prevolpac.ds.yml



nano sghi/datasets/fl_pep_st_evolucoes__prevolpac.ds.yml
## (ALTERAR A DATA)