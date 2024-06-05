## Trabalho Fundamentos de sistemas de informação

### Domínio de aplicação escolhido:     

#### Gestão de Ativos de TI na Empresa

**Indicador 1:** Percentual de máquinas alocadas por unidade

_Variáveis:_

* Número total de máquinas (TM)
* Número de máquinas por unidade (MU)
  Fórmula: MU / TM

**Indicador 2**: Percentual de usuários com Office atualizado

_Variáveis_:

* Número total de usuários (TU)
* Número de usuários com Office versão 2021 (UO)
  Fórmula: UO / TU

**Indicador 3**: Tempo médio de uso das máquinas por tipo

_Variáveis:_

* Data de alocação da máquina (DA)
* Data atual (DT)
  Fórmula: (DT - DA) / Número de máquinas (NM)

### Diagrama do modelo dimensional para cada indicador

**Indicador 1:** Percentual de máquinas alocadas por unidade
**Fato: Maquinas**
Medida: Contagem de máquinas
Dimensões:

* Unidade
* UnidadeID
* NomeUnidade
* Localizacao

**Indicador 2:** Percentual de usuários com Office atualizado
Fato: Usuários
Medida: Contagem de usuários com Office atualizado
Dimensões:

* Usuario

* UsuarioID
* NomeUsuario
* Email
* UnidadeID
* Office
* OfficeID
* NomeOffice
* Versao
* MaquinaID
* Ano

**Indicador 3:** Distribuição de tipos de máquinas por unidade
Fato: Maquinas
Medida: Contagem de máquinas por tipo
Dimensões:

* Unidade
* UnidadeID
* NomeUnidade
* Localizacao
* Maquina
* MaquinaID
* NomeMaquina
* Tipo
* UsuarioID
* SerialMaquina

![image](https://github.com/einstein808/trablhoFundTI/assets/79322072/9b258973-2619-4220-a0e5-c6369a71ca5d)


