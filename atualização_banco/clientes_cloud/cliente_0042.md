## CLIENTE 0042


**MODELO BASE — TODAS AS TABELAS**

## BANCO — 4

## RX — PRÉ-REQUISITO (caso não tenham rodado na rotina)
./ppa rxb -t atcabecatend
./ppa rxb -t ricadpac
./ppa rxb -t htatendimento
./ppa rxb -t  htpaciente


**Se está dentro de 24 horas - OK**


## 🔹 2. DIMENSÕES
 ./ppa dsb -s sghi/datasets/d_empresa__tbemphos.ds.yml
 ./ppa dsb -s sghi/datasets/d_unidade__tbunidad.ds.yml
 ./ppa dsb -s sghi/datasets/d_convenio__tbconven.ds.yml
 ./ppa dsb -s sghi/datasets/d_clinica__tbclinica.ds.yml
 ./ppa dsb -s sghi/datasets/d_especialidade__tbespec.ds.yml
 ./ppa dsb -s sghi/datasets/d_especialidade__tbesplei.ds.yml
 ./ppa dsb -s sghi/datasets/d_especialidade_exame__siespec.ds.yml
 ./ppa dsb -s sghi/datasets/d_exame__sitabpro.ds.yml
 ./ppa dsb -s sghi/datasets/d_servico_hospitalar__tbtabdth.ds.yml
 ./ppa dsb -s sghi/datasets/d_procedimento__tbprosus.ds.yml
 ./ppa dsb -s sghi/datasets/d_procedimento__tbtabthm.ds.yml
 ./ppa dsb -s sghi/datasets/d_material_medicamento__tbmatmed.ds.yml
 ./ppa dsb -s sghi/datasets/d_item_cobranca2__d_procedimento.ds.yml
 ./ppa dsb -s sghi/datasets/d_item_cobranca2__d_material_medicamento.ds.yml
 ./ppa dsb -s sghi/datasets/d_item_cobranca2__d_servico_hospitalar.ds.yml
 ./ppa dsb -s sghi/datasets/d_paciente__ricadpac.ds.yml
 ./ppa dsb -s sghi/datasets/d_perf_demografico__ricadpac.ds.yml
 ./ppa dsb -s sghi/datasets/d_ocupacao__tbcbosus.ds.yml
 ./ppa dsb -s sghi/datasets/d_motivo_alta__tbmotalt.ds.yml
 ./ppa dsb -s sghi/datasets/d_grupo_atendimento__tbgruate.ds.yml
 ./ppa dsb -s sghi/datasets/d_tipo_atendimento__tbiteate.ds.yml
 ./ppa dsb -s sghi/datasets/d_tipo_agendamento__retipage.ds.yml
 ./ppa dsb -s sghi/datasets/d_stt_agendamento__tbsitage.ds.yml
 ./ppa dsb -s sghi/datasets/d_leito__rileitos.ds.yml
 ./ppa dsb -s sghi/datasets/d_sala_cirurgica__ccsalas.ds.yml
 ./ppa dsb -s sghi/datasets/d_sala_cirurgica__ccsalas.ds.yml
 ./ppa dsb -s sghi/datasets/fa_ft_irregularidade__fiirregularid.ds.yml
 ./ppa dsb -s sghi/datasets/fa_ft_irregularidade__fcirregularid.ds.yml
 ./ppa dsb -s sghi/datasets/fa_ft_irregularidade__fcirregularid.ds.yml
 ./ppa dsb -s sghi/datasets/d_cid__tbcid10.ds.yml
 ./ppa dsb -s sghi/datasets/d_centro_custo__tbcencus.ds.yml
 ./ppa dsb -s sghi/datasets/d_conta_bancaria__tbbancos.ds.yml
 ./ppa dsb -s sghi/datasets/d_colaborador__getabfun.ds.yml
 ./ppa dsb -s sghi/datasets/d_prestador__tbprofis.ds.yml
 ./ppa dsb -s sghi/datasets/d_prestador__silanexa.ds.yml
 ./ppa dsb -s sghi/datasets/d_prestador2__tbmedsol.ds.yml
 ./ppa dsb -s sghi/datasets/d_prestador2__tbprofis.ds.yml
 ./ppa dsb -s sghi/datasets/d_favorecido_credor__tbfornec.ds.yml
 ./ppa dsb -s sghi/datasets/d_favorecido_credor__tbclient.ds.yml
 ./ppa dsb -s sghi/datasets/d_favorecido_credor__tbconven.ds.yml
 ./ppa dsb -s sghi/datasets/d_favorecido_credor__tbcooper.ds.yml
 ./ppa dsb -s sghi/datasets/d_favorecido_credor__tbinstituicaofin.ds.yml
 ./ppa dsb -s sghi/datasets/d_favorecido_credor__tborgaopublico.ds.yml
 ./ppa dsb -s sghi/datasets/d_favorecido_credor__tbprofis.ds.yml
 ./ppa dsb -s sghi/datasets/d_favorecido_credor__mflancto.ds.yml
 ./ppa dsb -s sghi/datasets/d_motivo_glosa__tbmotglo.ds.yml
 ./ppa dsb -s sghi/datasets/d_loc_armazena__gelocarm.ds.yml
 ./ppa dsb -s sghi/datasets/d_local_consumo__tbloccon.ds.yml
 ./ppa dsb -s sghi/datasets/d_plano_conta_contabil__coplano.ds.yml
 ./ppa dsb -s sghi/datasets/d_procedencia__tbproced.ds.yml
 ./ppa dsb -s sghi/datasets/d_produto__geitens.ds.yml
 ./ppa dsb -s sghi/datasets/d_terceiro__gecadter.ds.yml
 ./ppa dsb -s sghi/datasets/d_tp_custo_despesa__ctlancto.ds.yml
 ./ppa dsb -s sghi/datasets/d_usuario__tbusers.ds.yml

## 🔹 3. ATENDIMENTO

 ./ppa dsb -s sghi/datasets/f_at_aten_interno__ricadint.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_aten_externo__recadate.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_aten_externo__reexcate.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_mov_paciente__rictrloc.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_leito_dia__sghdw.ds.yml
 ./ppa dsb -s sghi/datasets/fa_at_fluxo_atendimento__tbfluxoatend.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_pesquisa_satisfacao__scentrev.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_inatividade_leito__riinalei.ds.yml

## 🔹 4. AGENDA E CIRURGIA

 ./ppa dsb -s sghi/datasets/f_at_agendamento__repacagd.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_agendamento__sipacagi.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_cirurgia__cclancir.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_cirurgia_agendada__ccagenda.ds.yml
 ./ppa dsb -s sghi/datasets/f_at_cirurgia_agendada__cchisage.ds.yml
 ./ppa dsb -s sghi/datasets/d_dados_cirurgia__cccadcir.ds.yml
 ./ppa dsb -s sghi/datasets/d_dados_parto__ccficpar.ds.yml

## 🔹 5. EXAMES E CUSTO

 ./ppa dsb -s sghi/datasets/f_at_exame__silanexa.ds.yml
 ./ppa dsb -s sghi/datasets/f_ct_custo__ctlancto.ds.yml
 ./ppa dsb -s sghi/datasets/f_ct_indicador__ctitepro.ds.yml

## 🔹 6. FINANCEIRO

 ./ppa dsb -s sghi/datasets/f_fi_movimento__mfconpag.ds.yml
 ./ppa dsb -s sghi/datasets/f_fi_movimento__mfctarec.ds.yml
 ./ppa dsb -s sghi/datasets/f_fi_movimento__mflancto.ds.yml
 ./ppa dsb -s sghi/datasets/f_fi_movimento__mfadifor.ds.yml
 ./ppa dsb -s sghi/datasets/f_fi_conta_saldo_dia__mflancto.ds.yml

## 🔹 7. FATURAMENTO

 ./ppa dsb -s sghi/datasets/f_ft_item_faturado__falansus.ds.yml
 ./ppa dsb -s sghi/datasets/f_ft_item_faturado__fhlancto.ds.yml
 ./ppa dsb -s sghi/datasets/f_ft_item_faturado__fhcondia.ds.yml
 ./ppa dsb -s sghi/datasets/f_ft_item_faturado.ds.yml
 ./ppa dsb -s sghi/datasets/d_dados_faturamento__factasus.ds.yml
 ./ppa dsb -s sghi/datasets/d_dados_faturamento__fclanext.ds.yml
 ./ppa dsb -s sghi/datasets/d_dados_faturamento__fhcadaih.ds.yml

## 🔹 8. SUPRIMENTOS / ESTOQUE

 ./ppa dsb -s sghi/datasets/f_sp_mov_produto__gelansai.ds.yml
 ./ppa dsb -s sghi/datasets/f_sp_mov_produto__gelandev.ds.yml
 ./ppa dsb -s sghi/datasets/f_sp_compra__gelannfs.ds.yml
 ./ppa dsb -s sghi/datasets/f_sp_saldo_estoque_dia__gesaldos.ds.yml
 ./ppa dsb -s sghi/datasets/f_sp_saldo_estoque_mes__sghdw.ds.yml
 ./ppa dsb -s sghi/datasets/f_sp_pedido_compra__gelanped.ds.yml
 ./ppa dsb -s sghi/datasets/fa_sp_consumo.ds.yml

## 🔹 9. PEP (ORDEM OBRIGATÓRIA)

 ./ppa dsb -s sghi/datasets/fl_pep_tmp__prevolpac.ds.yml
 ./ppa dsb -s sghi/datasets/fl_pep_st_evolucoes__prevolpac.ds.yml
 ./ppa dsb -s sghi/datasets/fl_pep_uevolucoes__prevolpac.ds.yml

## 🔹 10. CUSTOMIZADOS

 ./ppa dsb -s sghi/datasets/f_integra_bi.ds.yml
 ./ppa dsb -s sghi/datasets/f_rpa__rplaneve.ds.yml
 ./ppa dsb -s sghi/datasets/f_fp_resumo_folha2__fpfichaf.ds.yml
 ./ppa dsb -s sghi/datasets/bt_cdc_movimento__mfctarec.ds.yml
 ./ppa dsb -s sghi/datasets/bt_cdc_movimento__mfconpag.ds.yml
 ./ppa dsb -s sghi/datasets/bt_cdc_movimento__falansus.ds.yml
 ./ppa dsb -s sghi/datasets/bt_cdc_movimento__fclanext.ds.yml
 ./ppa dsb -s sghi/datasets/bt_cdc_movimento__rpa.ds.yml
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
---