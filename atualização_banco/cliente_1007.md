### CLIENTE 1007


**CASO NÃO TENHA ATUALIZADO NENHUMA, COMEÇAR LIMPANDO A MEMÓRIA**

./ppa kjb /rep:sghi /dir:job /job:vertica_maintenance_tasks
docker-compose stop rxb
docker-compose up -d rxb


**TABELAS**

./ppa rxb -t ricadpac
./ppa rxb -t htpaciente
./ppa rxb -t htatendimento
./ppa rxb -t htcid
./ppa rxb -t htleito
./ppa rxb -t atcabecatend
./ppa rxb -t ricadint
./ppa rxb -t recadate
./ppa rxb -t rictrloc
./ppa rxb -t repacagi
./ppa rxb -t repacagd
./ppa rxb -t sipacagi
./ppa rxb -t sipacagd
./ppa rxb -t prpergunta
./ppa rxb -t prresposta
./ppa rxb -t prevolucao
./ppa rxb -t prevolpac
./ppa rxb -t prcabevol
./ppa rxb -t cccadcir
./ppa rxb -t cclancir
./ppa rxb -t ccagenda
./ppa rxb -t cchisage
./ppa rxb -t sicadate
./ppa rxb -t silanexa
./ppa rxb -t ctlancto
./ppa rxb -t ctitepro
./ppa rxb -t mfconpag
./ppa rxb -t mfctarec
./ppa rxb -t mflancto
./ppa rxb -t fccctaext
./ppa rxb -t fclanext
./ppa rxb -t factasus
./ppa rxb -t falansus
./ppa rxb -t tbsubsus
./ppa rxb -t fhcadaih
./ppa rxb -t fhlancto
./ppa rxb -t fhaihemi
./ppa rxb -t fhcondia
./ppa rxb -t gecadsai
./ppa rxb -t gecadnnfs
./ppa rxb -t gelannfs
./ppa rxb -t gelansai
./ppa rxb -t gecaddev
./ppa rxb -t gelandev
./ppa rxb -t tbsenhaatend
./ppa rxb -t tbgerasenha
./ppa rxb -t tbfluxoatend



**Após processar as cargas manualmente, necessário realizar:**
./ppa kjb /rep:sghi /dir:job /job:vertica_maintenance_tasks

docker-compose stop rxb
docker-compose up -d rxb


